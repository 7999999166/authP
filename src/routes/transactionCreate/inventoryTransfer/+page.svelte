<script>
  // Inventory Transfer Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: #0077B6;">
      Inventory Transfer Form
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
                for="voucherNo"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher No</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control bg-light text-center fw-semibold"
                  id="voucherNo"
                  value="Auto Generated"
                  readonly
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="destinationWarehouse"
                class="col-4 col-form-label text-secondary fw-medium"
                >Destination Warehouse</label
              >
              <div class="col-8">
                <input
                  type="text"
                  class="form-control"
                  id="destinationWarehouse"
                />
              </div>
            </div>

            <div class="row align-items-center">
              <label
                for="voucherDate"
                class="col-4 col-form-label text-secondary fw-medium"
                >Voucher Date</label
              >
              <div class="col-8 position-relative">
                <input
                  type="text"
                  class="form-control"
                  id="voucherDate"
                  value="16 November 2025"
                />
                <span
                  class="position-absolute top-50 end-0 translate-middle-y me-3 text-secondary"
                >
                  <i class="bi bi-calendar"></i>
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="d-flex align-items-end gap-4 mb-4">
        <div class="flex-grow-1">
          <label for="f9Item" class="fw-medium text-secondary mb-2 d-block"
            >F9: Item</label
          >
          <input type="text" class="form-control" id="f9Item" />
          <small class="text-secondary d-block mt-1"
            >Press ENTER key to add. ESCAPE to leave.</small
          >
        </div>
        <div class="d-flex align-items-center gap-3 pb-2">
          <span class="fw-medium text-secondary">Units</span>
          <a href="#" class="text-primary text-decoration-none small"
            >Alt+F1: Warehouse Units</a
          >
        </div>
      </div>

      <div class="table-responsive border border-secondary-subtle rounded">
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium">Item</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Source Warehouse</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Quantity</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Rate/Unit</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Amount</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="5" class="text-center text-secondary py-5">
                No items added.
              </td>
            </tr>
          </tbody>
        </table>
      </div>
      <small class="text-secondary d-block mt-2"
        >Press DELETE key to remove item row. Use ENTER to move forward &
        SHIFT+ENTER to move back within the table.</small
      >
    </div>

    <!-- Bottom Section -->
    <div class="row g-4 align-items-end">
      <div class="col-md-6">
        <label for="narration" class="fw-medium text-secondary mb-2"
          >Narration</label
        >
        <textarea class="form-control" id="narration" rows="3"></textarea>
        <small class="text-secondary d-block mt-1"
          >Use Ctrl+Enter for next line</small
        >
      </div>

      <div class="col-md-6 d-flex justify-content-end align-items-center gap-3">
        <label for="totalValue" class="fw-medium text-secondary"
          >Total Value</label
        >
        <input
          type="text"
          class="form-control bg-light text-end fw-semibold"
          id="totalValue"
          value="0"
          readonly
          style="width: 160px;"
        />
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium">
        Ctrl+Q: Exit
      </button>
      <a
        href="#"
        class="btn btn-light border text-secondary fw-medium text-decoration-none"
      >
        Video: How to Transfer Stock?
      </a>
    </div>
    <button class="btn btn-primary fw-medium"> F12:Save </button>
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
