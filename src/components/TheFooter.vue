<template>
  <footer class="border-top vultive-bg-muted">
    <div class="container-sm">
      <div class="row py-5">
        <div class="col-md-4" id="company">
          <h3>Company</h3>
          <ul class="pt-2">
            <li>
              <a href="/static/pdfs/termsandconditions.pdf"
                >Terms and conditions</a
              >
            </li>
            <li>
              <a href="/static/pdfs/privacypolicy.pdf">Privacy policy</a>
            </li>
          </ul>
        </div>
        <div class="col-md-4" id="contact">
          <h3>Contact</h3>
          <ul class="pt-2">
            <li>
              Email:
              <a class="fw-bold" href="mailto: support@vultive.com"
                >support@vultive.com</a
              >
            </li>
          </ul>
        </div>
        <div class="col-md-4">
          <a
            class="twitter-timeline"
            data-height="250"
            data-theme="light"
            href="https://twitter.com/vultivecom"
            >Twitter</a
          >
        </div>
      </div>
      <div class="py-3 fs-6">© 2022 Vultive Team. All Rights Reserved.</div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Components - TheFooter",
};
</script>
