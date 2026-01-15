<script>
  // Inventory Adjustment Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: var(--btn-primary);">
      Inventory Adjustment Form
    </h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-md-4">
          <div class="d-flex flex-column gap-3">
            <div class="d-flex flex-column gap-1">
              <label for="voucherNo" class="fw-medium text-secondary"
                >Voucher No</label
              >
              <input
                type="text"
                class="form-control bg-white"
                id="voucherNo"
                value="Auto Generated"
                readonly
              />
            </div>

            <div class="d-flex flex-column gap-1">
              <label for="voucherDate" class="fw-medium text-secondary"
                >Voucher Date</label
              >
              <div class="position-relative">
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

        <div class="col-md-4"></div>

        <div class="col-md-4">
          <div class="border border-secondary-subtle rounded p-3">
            <p class="fw-medium text-secondary mb-2">Adjustment Type</p>
            <div class="d-flex gap-4">
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="adjustmentType"
                  id="addStock"
                  checked
                />
                <label class="form-check-label text-dark small" for="addStock"
                  >Add Stock</label
                >
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="adjustmentType"
                  id="reduceStock"
                />
                <label
                  class="form-check-label text-dark small"
                  for="reduceStock">Reduce Stock</label
                >
              </div>
            </div>
          </div>
          <div class="form-check mt-3">
            <input class="form-check-input" type="checkbox" id="manualAdjust" />
            <label
              class="form-check-label text-secondary small"
              for="manualAdjust">Enter Physical Stock Manually To Adjust</label
            >
          </div>
        </div>
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row align-items-end mb-4 g-3">
        <div class="col-md-6">
          <label for="item" class="fw-medium text-secondary mb-1"
            >F9: Item</label
          >
          <input type="text" class="form-control" id="item" />
          <small class="text-secondary d-block mt-1"
            >Press ENTER key to add. ESCAPE to leave.</small
          >
        </div>
        <div class="col-md-6">
          <small class="text-secondary d-block"
            >Press DELETE key to remove item row.</small
          >
          <small class="text-secondary d-block"
            >Press ENTER to move forward & SHIFT-ENTER to move back.</small
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
    </div>

    <!-- Bottom Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <div class="col-md-8">
          <label for="narration" class="fw-medium text-secondary mb-1"
            >Narration</label
          >
          <textarea class="form-control" id="narration" rows="4"></textarea>
          <small class="text-secondary d-block mt-1"
            >Use Ctrl+Enter for next line</small
          >
          <a
            href="#"
            class="text-primary text-decoration-none small mt-2 d-block"
            >Video: Inventory Adjustment: Add/Reduce Stock</a
          >
        </div>

        <div
          class="col-md-4 d-flex flex-column justify-content-end align-items-end"
        >
          <div class="d-flex align-items-center gap-2">
            <label for="totalValue" class="fw-medium text-secondary"
              >Total Value</label
            >
            <input
              type="text"
              class="form-control bg-light text-center fw-semibold"
              id="totalValue"
              value="0.00"
              readonly
              style="width: 160px;"
            />
          </div>
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
