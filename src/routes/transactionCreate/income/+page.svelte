<script>
  // Receipt Entry Form (Income)
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: var(--btn-primary);">
      Receipt Entry Form
    </h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-md-6">
          <div class="d-flex flex-column gap-3">
            <div class="row align-items-center">
              <label
                for="receipt-no"
                class="col-4 col-form-label text-secondary fw-medium"
                >Receipt No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-light"
                  id="receipt-no"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

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
                  value="16 November 2025"
                />
                <span
                  class="position-absolute top-50 end-0 translate-middle-y me-3 text-secondary"
                >
                  <i class="bi bi-calendar"></i>
                </span>
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="received-into"
                class="col-4 col-form-label text-secondary fw-medium"
                >Received Into</label
              >
              <div class="col-8">
                <input type="text" class="form-control" id="received-into" />
                <small class="text-primary d-block mt-1">balance</small>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-6 d-flex flex-column justify-content-end">
          <div class="row align-items-start">
            <label
              for="received-from"
              class="col-4 col-form-label text-secondary fw-medium pt-2"
              >F9: Received From</label
            >
            <div class="col-8">
              <small class="text-secondary d-block mb-1"
                >Press ENTER key to add.</small
              >
              <input type="text" class="form-control" id="received-from" />
              <small class="text-primary d-block mt-1">balance</small>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <small class="text-secondary d-block mb-3"
        >Press ENTER to move forward & SHIFT+ENTER to move back.</small
      >

      <div class="table-responsive border border-secondary-subtle rounded">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium"
                >Account</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Amount</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="2" class="text-center text-secondary py-5">
                No entries added yet.
              </td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="d-flex justify-content-end align-items-center mt-3 gap-3">
        <label for="total" class="fw-medium text-secondary">Total</label>
        <input
          type="text"
          class="form-control bg-light text-end fw-semibold"
          id="total"
          value="0.00"
          readonly
          style="width: 150px;"
        />
      </div>
    </div>

    <!-- Narration -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row">
        <label
          for="narration"
          class="col-md-3 col-form-label fw-medium text-secondary"
          >Narration</label
        >
        <div class="col-md-9">
          <textarea class="form-control" id="narration" rows="3"></textarea>
          <small class="text-secondary d-block mt-1"
            >Use Ctrl+Enter for next line</small
          >
        </div>
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium p-2">
        <i class="bi bi-calculator"></i>
      </button>
      <button class="btn btn-light border text-secondary fw-medium">
        Alt+F12: Save & View
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
