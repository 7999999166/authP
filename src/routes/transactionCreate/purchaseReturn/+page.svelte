<script>
  // Purchase Return Form
</script>

<div class="container-fluid min-vh-100 d-flex flex-column p-4">
  <!-- Header -->
  <header class="mb-4">
    <h1 class="h3 fw-bold text-primary">Purchase Return</h1>
  </header>

  <main class="flex-grow-1 d-flex flex-column gap-4">
    <!-- Top Section -->
    <div class="border border-secondary-subtle p-4 rounded bg-transparent">
      <div class="row g-4">
        <!-- Debit Note No -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label
              for="debitNoteNo"
              class="col-4 col-form-label text-secondary fw-medium"
              >Debit Note No</label
            >
            <div class="col-8">
              <input
                type="text"
                class="form-control bg-light text-secondary"
                id="debitNoteNo"
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

        <!-- Supplier/Cash -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-start">
            <label
              for="supplier"
              class="col-4 col-form-label text-secondary fw-medium pt-2"
              >Supplier/Cash</label
            >
            <div class="col-8">
              <input type="text" class="form-control" id="supplier" />
              <small class="text-secondary d-block mt-1">balance</small>
            </div>
          </div>
        </div>

        <!-- Credit Account -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-start">
            <label
              for="creditAccount"
              class="col-4 col-form-label text-secondary fw-medium pt-2"
              >Credit Account</label
            >
            <div class="col-8">
              <input
                type="text"
                class="form-control"
                id="creditAccount"
                value="Purchases Return"
              />
              <small class="text-secondary d-block mt-1">balance</small>
            </div>
          </div>
        </div>

        <!-- Location Type -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label class="col-4 col-form-label text-secondary fw-medium"
              >Location</label
            >
            <div class="col-8 d-flex align-items-center gap-3">
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="locationType"
                  id="local"
                  checked
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="local">Local</label
                >
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="locationType"
                  id="interstate"
                />
                <label
                  class="form-check-label text-secondary fw-medium"
                  for="interstate">Interstate</label
                >
              </div>
              <input
                type="text"
                class="form-control form-control-sm text-center bg-light"
                value="DEFAULT"
                readonly
                style="width: 80px;"
              />
            </div>
          </div>
        </div>

        <!-- Place of Supply -->
        <div class="col-lg-4 col-md-6">
          <div class="row align-items-center">
            <label
              for="placeOfSupply"
              class="col-4 col-form-label text-secondary fw-medium"
              >Place Of Supply</label
            >
            <div class="col-8">
              <select class="form-select" id="placeOfSupply">
                <option>Delhi</option>
                <option>Mumbai</option>
                <option>Kolkata</option>
              </select>
            </div>
          </div>
        </div>
      </div>

      <!-- Helper Text -->
      <div class="mt-3 text-center">
        <span class="small fw-medium text-secondary"
          >Press ENTER to move forward</span
        >
      </div>
    </div>

    <!-- Item Entry & Table Section -->
    <div
      class="border border-secondary-subtle p-4 rounded bg-transparent d-flex flex-column flex-grow-1"
      style="min-height: 400px;"
    >
      <!-- Item Inputs -->
      <div class="row mb-4 g-4">
        <div class="col-md-6">
          <div class="d-flex align-items-center gap-2 mb-1">
            <label
              for="f9item"
              class="fw-medium text-secondary"
              style="width: 80px;">F9: Item</label
            >
            <input type="text" class="form-control" id="f9item" />
          </div>
          <div class="d-flex justify-content-between small ps-5 ms-4">
            <span class="text-secondary">Units Left: 0</span>
            <a href="#" class="text-primary text-decoration-none"
              >Alt+F1: Warehouse</a
            >
          </div>
          <div class="mt-2 small text-danger fw-medium">
            Press ENTER key to add item.
          </div>
        </div>

        <div class="col-md-6">
          <div class="d-flex align-items-center gap-2 mb-1">
            <label
              for="f10service"
              class="fw-medium text-secondary"
              style="width: 100px;">F10: Service</label
            >
            <input type="text" class="form-control" id="f10service" />
          </div>
          <div class="mt-2 small text-danger fw-medium text-end">
            DELETE: To Delete Row, Shift+UP/Down: To Rearrange Items
          </div>
        </div>
      </div>

      <!-- Table -->
      <div
        class="table-responsive border border-secondary-subtle rounded flex-grow-1"
      >
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
                >Value</th
              >
              <th class="small text-secondary text-uppercase fw-medium"
                >Description</th
              >
            </tr>
          </thead>
          <tbody>
            <tr>
              <td colspan="8" class="text-center text-secondary py-5">
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
      <div class="col-md-4">
        <div class="d-flex flex-column gap-3">
          <button class="btn btn-light border w-100 text-start fw-medium">
            Set off against purchase
          </button>

          <div class="d-flex flex-column gap-2">
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="tax" />
              <label class="form-check-label fw-medium text-secondary" for="tax"
                >Tax</label
              >
            </div>
            <div class="form-check">
              <input
                class="form-check-input"
                type="checkbox"
                id="otherCharges"
              />
              <label
                class="form-check-label fw-medium text-secondary"
                for="otherCharges">Other Charges</label
              >
            </div>
            <div class="form-check">
              <input class="form-check-input" type="checkbox" id="dispatch" />
              <label
                class="form-check-label fw-medium text-secondary"
                for="dispatch">Dispatch</label
              >
            </div>
          </div>
        </div>
      </div>

      <!-- Narration -->
      <div class="col-md-4">
        <div class="d-flex flex-column gap-2">
          <label for="narration" class="fw-medium text-secondary"
            >Narration</label
          >
          <textarea class="form-control" id="narration" rows="4"></textarea>
          <small class="text-secondary">Ctrl+Enter for next line</small>
        </div>
      </div>

      <!-- Totals -->
      <div class="col-md-4">
        <div class="d-flex flex-column gap-3">
          <div class="d-flex align-items-center justify-content-end gap-3">
            <label for="amount" class="fw-medium text-secondary">Amount</label>
            <input
              type="text"
              class="form-control bg-light text-end fw-medium"
              id="amount"
              value="0"
              readonly
              style="width: 150px;"
            />
          </div>

          <div class="border border-secondary-subtle p-3 rounded">
            <div class="d-flex align-items-center justify-content-between mb-3">
              <label for="roundOff" class="fw-medium text-secondary"
                >Round Off</label
              >
              <input
                type="text"
                class="form-control text-end"
                id="roundOff"
                value="0.00"
                style="width: 150px;"
              />
            </div>
            <div class="d-flex align-items-center justify-content-between">
              <label for="totalAmount" class="fw-bold text-secondary"
                >Total Amount</label
              >
              <input
                type="text"
                class="form-control bg-light text-end fw-bold fs-5"
                id="totalAmount"
                value="0.00"
                readonly
                style="width: 150px;"
              />
            </div>
          </div>

          <div class="border border-secondary-subtle p-3 rounded">
            <label class="fw-semibold text-secondary d-block mb-2"
              >Discount & Tax</label
            >
            <div class="d-flex gap-3">
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="discountType"
                  id="onTotal"
                  checked
                />
                <label class="form-check-label text-secondary" for="onTotal"
                  >On Total</label
                >
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="radio"
                  name="discountType"
                  id="perItem"
                />
                <label class="form-check-label text-secondary" for="perItem"
                  >Per Item</label
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer Action Bar -->
  <footer
    class="mt-5 pt-3 border-top border-secondary-subtle d-flex justify-content-between align-items-center sticky-bottom bg-background-light z-1 p-3 mx-n4 mb-n4"
  >
    <button class="btn btn-light border text-secondary fw-medium">
      Ctrl+Q: Exit
    </button>
    <div class="d-flex gap-2">
      <button class="btn btn-light border text-secondary fw-medium">
        Save & View
      </button>
      <button
        class="btn btn-primary d-flex align-items-center gap-1 fw-medium shadow-sm"
      >
        F12: Save
        <i class="bi bi-chevron-right small"></i>
      </button>
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
