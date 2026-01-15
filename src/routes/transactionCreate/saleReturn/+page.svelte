<script>
  // Sale Return Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold mb-4" style="color: var(--btn-primary);">
      Sale Return Form
    </h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <!-- Credit Note No -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label
              for="credit-note-no"
              class="col-4 col-form-label text-secondary fw-medium"
              >Credit Note No</label
            >
            <div class="col-8">
              <input
                type="text"
                class="form-control bg-light text-secondary"
                id="credit-note-no"
                value="Auto Generated"
                readonly
              />
            </div>
          </div>
        </div>

        <!-- Voucher Date -->
        <div class="col-lg-4 col-md-6">
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
        </div>

        <!-- Debit Account -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label
              for="debit-account"
              class="col-4 col-form-label text-secondary fw-medium"
              >Debit Account</label
            >
            <div class="col-8">
              <input
                type="text"
                class="form-control"
                id="debit-account"
                value="Sales Return"
              />
            </div>
          </div>
        </div>

        <!-- Customer/Cash -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-start">
            <label
              for="customer-cash"
              class="col-4 col-form-label text-secondary fw-medium pt-2"
              >Customer/Cash</label
            >
            <div class="col-8">
              <input type="text" class="form-control" id="customer-cash" />
              <small class="text-secondary d-block mt-1">balance</small>
            </div>
          </div>
        </div>

        <!-- Location -->
        <div class="col-lg-4 col-md-6">
          <div class="d-flex align-items-center gap-3 h-100">
            <div class="form-check mb-0">
              <input
                class="form-check-input"
                type="radio"
                name="location"
                id="local"
                checked
              />
              <label
                class="form-check-label text-secondary fw-medium"
                for="local">Local</label
              >
            </div>
            <div class="form-check mb-0">
              <input
                class="form-check-input"
                type="radio"
                name="location"
                id="interstate"
              />
              <label
                class="form-check-label text-secondary fw-medium"
                for="interstate">Interstate</label
              >
            </div>
            <input
              type="text"
              class="form-control form-control-sm text-center bg-light ms-auto"
              value="DEFAULT"
              readonly
              style="width: 100px;"
            />
          </div>
        </div>

        <!-- Place of Supply -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label
              for="place-of-supply"
              class="col-4 col-form-label text-secondary fw-medium text-end"
              >Place Of Supply</label
            >
            <div class="col-8">
              <select class="form-select" id="place-of-supply">
                <option selected>Delhi</option>
                <option>Mumbai</option>
                <option>Kolkata</option>
              </select>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div
      class="border border-secondary-subtle p-4 rounded bg-transparent d-flex flex-column flex-grow-1"
      style="min-height: 400px;"
    >
      <!-- Item Inputs -->
      <div class="row mb-4 g-4">
        <div class="col-md-8">
          <label for="f9-item" class="form-label fw-medium text-secondary"
            >F9: Item</label
          >
          <small class="text-secondary d-block mb-2"
            >Press ENTER key to add item. Press ENTER to move forward</small
          >
          <input type="text" class="form-control" id="f9-item" />
          <div class="d-flex gap-3 mt-2 small">
            <span class="text-secondary">Units Left: 0</span>
            <a href="#" class="text-primary text-decoration-none"
              >Alt+F1: Warehouse</a
            >
          </div>
        </div>

        <div class="col-md-4">
          <label for="f10-service" class="form-label fw-medium text-secondary"
            >F10: Service</label
          >
          <small class="text-secondary d-block mb-2 invisible"
            >Placeholder</small
          >
          <input type="text" class="form-control" id="f10-service" />
        </div>
      </div>

      <!-- Table -->
      <div
        class="table-responsive border-top border-secondary-subtle pt-3 flex-grow-1"
      >
        <div class="d-flex justify-content-end mb-2">
          <small class="text-secondary"
            >DELETE: To Delete Row, Shift+UP/Down: To Rearrange Items</small
          >
        </div>
        <table class="table table-hover mb-0">
          <thead class="table-light">
            <tr>
              <th class="small text-secondary text-uppercase fw-medium">Item</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Warehouse</th
              >
              <th class="small text-secondary text-uppercase fw-medium">QTY</th>
              <th class="small text-secondary text-uppercase fw-medium"
                >Units</th
              >
              <th class="small text-secondary text-uppercase fw-medium">Rate</th
              >
              <th class="small text-secondary text-uppercase fw-medium">Per</th>
              <th class="small text-secondary text-uppercase fw-medium"
                >Discount(%)</th
              >
              <th class="small text-secondary text-uppercase fw-medium">Tax</th>
              <th class="small text-secondary text-uppercase fw-medium"
                >Value</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Description</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="10" class="text-center text-secondary py-5">
                No items added.
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <!-- Bottom Section -->
    <div class="row g-4">
      <!-- Options -->
      <div class="col-lg-4">
        <div class="d-flex flex-column gap-3">
          <button class="btn btn-light border w-100 text-start fw-medium">
            Set off against invoice
          </button>

          <div class="d-flex align-items-center gap-2">
            <input
              class="form-check-input"
              type="checkbox"
              id="other-charges"
            />
            <label
              class="form-check-label fw-medium text-secondary"
              for="other-charges">Other Charges</label
            >
          </div>

          <div>
            <label for="narration" class="form-label fw-medium text-secondary"
              >Narration</label
            >
            <textarea class="form-control" id="narration" rows="3"></textarea>
            <small class="text-secondary d-block mt-1"
              >Ctrl+Enter for next line</small
            >
          </div>

          <div class="d-flex align-items-center gap-2">
            <input class="form-check-input" type="checkbox" id="dispatch" />
            <label
              class="form-check-label fw-medium text-secondary"
              for="dispatch">Dispatch</label
            >
          </div>
        </div>
      </div>

      <!-- Totals -->
      <div class="col-lg-8">
        <div class="d-flex flex-column align-items-end gap-3">
          <div class="d-flex align-items-center gap-3">
            <label for="amount" class="fw-medium text-secondary">Amount</label>
            <input
              type="text"
              class="form-control bg-light text-end fw-semibold"
              id="amount"
              value="0"
              readonly
              style="width: 150px;"
            />
          </div>

          <div
            class="border border-secondary-subtle p-3 rounded w-100"
            style="max-width: 400px;"
          >
            <div class="d-flex align-items-center justify-content-between mb-3">
              <label for="round-off" class="fw-medium text-secondary"
                >Round Off</label
              >
              <input
                type="text"
                class="form-control text-end"
                id="round-off"
                value="0.00"
                style="width: 150px;"
              />
            </div>

            <div>
              <label class="fw-medium text-secondary d-block mb-2 text-end"
                >Discount & Tax</label
              >
              <div class="d-flex justify-content-end gap-3">
                <div class="form-check">
                  <input
                    class="form-check-input"
                    type="radio"
                    name="discount-tax"
                    id="on-total"
                    checked
                  />
                  <label class="form-check-label text-secondary" for="on-total"
                    >On Total</label
                  >
                </div>
                <div class="form-check">
                  <input
                    class="form-check-input"
                    type="radio"
                    name="discount-tax"
                    id="per-item"
                  />
                  <label class="form-check-label text-secondary" for="per-item"
                    >Per Item</label
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="d-flex align-items-center gap-3">
            <label for="total-amount" class="fw-bold text-secondary"
              >Total Amount</label
            >
            <input
              type="text"
              class="form-control text-end fw-bold"
              id="total-amount"
              value="0.00"
              style="width: 150px;"
            />
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer Action Bar -->
  <footer
    class="mt-4 pt-4 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <button
      class="btn btn-primary d-flex align-items-center gap-1 fw-medium shadow-sm"
    >
      F12:Save
    </button>
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
