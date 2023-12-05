<template>
  <div class="bg-green-50 page-section py-5">
    <div class="container">
      <div class="text-center wow fadeInUp">
        <div class="mt-2 subhead">Precios</div>
        <h2 class="title-section">
          Mira los ultimos
          <span class="">Precios</span>
        </h2>
        <div class="divider mx-auto"></div>
      </div>

      <div class="row my-5   p-5">
         
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm">
              <div class="card-header py-3">
                <h4 class="my-0 fw-normal">Free</h4>
              </div>
              <div class="card-body">
                <h1 class="card-title pricing-card-title">$0<small class="text-body-secondary fw-light">/mo</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  <li>10 users included</li>
                  <li>2 GB of storage</li>
                  <li>Email support</li>
                  <li>Help center access</li>
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-outline-primary">Sign up for free</button>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm">
              <div class="card-header py-3">
                <h4 class="my-0 fw-normal">Pro</h4>
              </div>
              <div class="card-body">
                <h1 class="card-title pricing-card-title">$15<small class="text-body-secondary fw-light">/mo</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  <li>20 users included</li>
                  <li>10 GB of storage</li>
                  <li>Priority email support</li>
                  <li>Help center access</li>
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-primary">Get started</button>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm border-success">
              <div class="card-header py-3 text-bg-success border-success">
                <h4 class="my-0 fw-normal">Enterprise</h4>
              </div>
              <div class="card-body">
                <h1 class="card-title pricing-card-title">$29<small class="text-body-secondary fw-light">/mo</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  <li>30 users included</li>
                  <li>15 GB of storage</li>
                  <li>Phone and email support</li>
                  <li>Help center access</li>
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-primary">Contact us</button>
              </div>
            </div>
          </div>
 
         
      </div>

      <div class="text-center pb-5">
        <router-link
          to="https://vueblog-13514.web.app/"
          class="btn btn-outline-primary rounded-pill">
          Discover More
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    blog: Array,
  },
};
</script>

<style></style>
