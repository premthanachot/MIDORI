<template>
  <div>
    <header
      class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm"
    >
      <p class="h3 my-0 me-md-auto fw-normal">MIDORI-SHOP</p>
      <a class="btn btn-outline-primary">µÃÐ¡ÃéÒÊÔ¹¤éÒ</a>
    </header>
    <main class="container">
      <div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
        <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i1.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i1.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i1.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-1">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i1.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i1.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i2.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i2.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i2.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-2">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i2.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i2.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i3.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i3.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i3.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-3">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i3.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i3.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i4.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i4.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i4.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-1">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i4.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i4.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i5.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i5.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i5.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-2">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i5.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i5.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i6.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i6.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i6.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-3">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i6.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i6.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i7.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i7.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i7.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-1">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i7.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i7.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i8.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i8.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i8.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-2">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i8.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i8.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i9.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i9.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i9.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-3">
                  <i class="bi bi-patch-plus"></i>
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i9.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i9.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i1.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i10.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i10.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-1">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i10.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i10.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i11.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i11.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i11.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-2">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i11.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i11.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ $store.state.i12.name }}</h4>
              </div>
              <div class="card-body">
                <img :src="$store.state.i12.image" width="240" />
                <ul class="list-unstyled text-small">
                  {{
                    $store.state.i12.price
                  }}
                  ºÒ·
                </ul>
                <div id="example-3">
                  <button
                    type="button"
                    class="w-100 btn btn-lg btn-outline-primary"
                    v-on:click="
                      ($store.state.i12.amount += 1),
                        $store.state.say(
                          'à¾ÔèÁÊÔ¹¤éÒÊÓàÃç¨ ÊÒÁÒÃ¶µÃÇ¨ÊÍºá¡éä¢ÊÔ¹¤éÒä´éã¹µÃÐ¡ÃéÒ'
                        )
                    "
                  >
                    à¾ÔèÁÊÔ¹¤éÒ
                  </button>
                  <p>¨Ó¹Ç¹ {{ $store.state.i12.amount }} à«çµ</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>
