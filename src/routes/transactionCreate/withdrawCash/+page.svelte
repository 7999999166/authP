<script>
  // Withdraw Cash Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-0">
  <div class="flex-grow-1 p-4">
    <div class="container-fluid p-0" style="max-width: 1280px;">
      <h1 class="h3 fw-bold mb-4" style="color: var(--btn-primary);">
        Withdraw Cash
      </h1>

      <div
        class="border border-secondary-subtle rounded p-4 mb-4 bg-background-light"
      >
        <div class="row g-4">
          <!-- Left Column -->
          <div class="col-lg-4 col-md-6 d-flex flex-column gap-3">
            <!-- Contra No -->
            <div class="row align-items-center">
              <label
                for="contra-no"
                class="col-4 col-form-label text-secondary fw-medium"
                >Contra No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="contra-no"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

            <!-- Voucher Date -->
            <div class="row align-items-center">
              <label
                for="voucher-date"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher Date</label
              >
              <div class="col-8 position-relative">
                <input
                  type="text"
                  class="form-control"
                  id="voucher-date"
                  value="06 November 2025"
                />
                <span
                  class="position-absolute top-50 end-0 translate-middle-y me-3 text-secondary"
                >
                  <i class="bi bi-calendar"></i>
                </span>
              </div>
            </div>

            <!-- To Account -->
            <div class="row align-items-center">
              <label
                for="to-account"
                class="col-4 col-form-label text-secondary fw-medium"
                >To Account</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="to-account"
                  value="Cash"
                />
                <small class="text-secondary d-block mt-1">balance</small>
              </div>
            </div>

            <!-- From Account -->
            <div class="row align-items-center">
              <label
                for="from-account"
                class="col-4 col-form-label text-secondary fw-medium"
                >From Account</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="from-account" />
                <div class="d-flex justify-content-between mt-1 small">
                  <span class="text-secondary">balance</span>
                  <span class="text-dark fw-medium">-1,18,55,123.53</span>
                </div>
              </div>
            </div>
          </div>

          <!-- Middle Column (Spacer) -->
          <div class="col-lg-4 d-none d-lg-block"></div>

          <!-- Right Column -->
          <div
            class="col-lg-4 col-md-6 d-flex flex-column justify-content-between"
          >
            <div class="d-flex flex-column gap-3">
              <!-- Amount -->
              <div class="row align-items-center">
                <label
                  for="amount"
                  class="col-4 col-form-label text-secondary fw-medium"
                  >Amount</label
                >
                <div class="col-8">
                  <input
                    type="text"
                    class="form-control text-end"
                    id="amount"
                    value="0"
                  />
                </div>
              </div>

              <!-- Total Amount -->
              <div class="row align-items-center">
                <label
                  for="total-amount"
                  class="col-4 col-form-label text-secondary fw-medium"
                  >Total Amount</label
                >
                <div class="col-8">
                  <input
                    type="text"
                    class="form-control bg-light text-end fw-semibold"
                    id="total-amount"
                    value="0.00"
                    readonly
                  />
                </div>
              </div>
            </div>
            <div class="text-end mt-3">
              <small class="text-secondary">Press ENTER to move forward</small>
            </div>
          </div>

          <!-- Narration (Full Width) -->
          <div class="col-12">
            <label for="narration" class="form-label fw-medium text-secondary"
              >Narration</label
            >
            <textarea class="form-control" id="narration" rows="4"></textarea>
            <small class="text-secondary d-block mt-1"
              >Ctrl+Enter for next line</small
            >
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer
    class="border-top border-secondary-subtle mt-auto sticky-bottom bg-background-light"
  >
    <div
      class="container-fluid px-4 py-3 d-flex justify-content-between align-items-center"
      style="max-width: 1280px;"
    >
      <button class="btn btn-light border text-secondary fw-medium">
        Ctrl+Q: Exit
      </button>
      <button class="btn btn-primary fw-medium"> F12: Save </button>
    </div>
  </footer>
</div>

<style>
  .bg-background-light {
    background-color: var(--background-light);
  }
  .form-control,
  .form-select {
    padding: 0.5rem 0.75rem;
  }
</style>
