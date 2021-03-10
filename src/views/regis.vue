<template>
  <div id="login">
    <b-container>
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
      <b-card bg-variant="secondary" text-variant="white" title="Register">
        <b-form @submit="onSubmit" @reset="onReset" v-if="show">
          <b-form-group
            id="input-group-1"
            label="Email address:"
            label-for="input-1"
            description="We'll never share your email with anyone else."
          >
            <b-form-input
              id="input-1"
              v-model="form.email"
              type="email"
              placeholder="Enter Email"
              required
            ></b-form-input>
          </b-form-group>
          <b-row>
            <b-col cols="6">
              <b-form-group
                id="input-group-2"
                label="Name:"
                label-for="input-2"
              >
                <b-form-input
                  id="input-2"
                  v-model="form.name"
                  placeholder="Enter Name"
                  required
                ></b-form-input>
              </b-form-group>
            </b-col>
            <b-col cols="6">
              <b-form-group
                id="input-group-3"
                label="Surname:"
                label-for="input-3"
              >
                <b-form-input
                  id="input-3"
                  v-model="form.surname"
                  placeholder="Enter Surname"
                  required
                ></b-form-input>
              </b-form-group>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="6">
              <b-form-group
                id="input-group-7"
                label="Password:"
                label-for="input-7"
              >
                <b-form-input
                  id="input-7"
                  v-model="form.pass"
                  placeholder="Enter your password"
                  required
                ></b-form-input>
              </b-form-group>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="6">
              <b-form-group
                id="input-group-4"
                label="Phone:"
                label-for="input-4"
              >
                <b-form-input
                  id="input-4"
                  v-model="form.phone"
                  placeholder="Enter your phone"
                  required
                ></b-form-input>
              </b-form-group>
            </b-col>
            <b-col cols="6">
              <b-form-group
                id="input-group-5"
                label="Gender:"
                label-for="input-5"
              >
                <b-form-select
                  id="input-5"
                  v-model="form.gender"
                  :options="gender"
                  required
                ></b-form-select>
              </b-form-group>
            </b-col>
          </b-row>
          <b-button type="submit" variant="primary">Submit</b-button>
          <b-button variant="success">Google</b-button>
          <b-button type="reset" variant="danger">Reset</b-button>
        </b-form>
        <!-- <b-card class="mt-3" header="Form Data Result">
      <pre class="m-0">{{ form }}</pre>
    </b-card> -->
      </b-card>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: "",
        name: "",
        surname: "",
        phone: "",
        food: null,
      },
      gender: [{ text: "Select One", value: null }, "Male", "Female", "Other"],
      show: true,
    };
  },
  methods: {
    onSubmit(event) {
      event.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset(event) {
      event.preventDefault();
      // Reset our form values
      this.form.email = "";
      this.form.name = "";
      this.form.surname = "";
      this.form.phone = "";
      this.form.gender = null;
      this.form.pass = "";
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>
