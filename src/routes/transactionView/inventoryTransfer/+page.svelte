<script>
  // Transaction View: Inventory Transfer (Stock Journal)
  // Layout based on inventoryTransfer/stock journal.png
</script>

<div class="container-fluid bg-white p-4 min-vh-100 font-monospace">
  <!-- Header -->
  <div class="text-center mb-4">
    <h4 class="fw-bold mb-1">
      AKHIL STAINLESS STEEL INDUSTRIES PRIVATE LIMITED
    </h4>
    <p class="mb-0 small">
      KH No. 93/13, Mundka Industrial Area, New Delhi -110041
    </p>
    <p class="mb-0 small">
      <i class="bi bi-envelope me-1"></i>assipl023@gmail.com,
      <i class="bi bi-telephone me-1"></i>9999995595
    </p>
    <p class="mb-0 small fw-bold">GSTIN: 07AAYCA5420B1ZS</p>
  </div>

  <!-- Box -->
  <div class="border border-dark mb-0">
    <!-- Title Row -->
    <div class="d-flex justify-content-end p-2 border-bottom border-dark">
      <div class="text-end">
        <h2 class="fw-bold mb-1">Stock Journal</h2>
        <div class="mb-1">
          <span class="fw-bold">Stock Journal No:</span> STK2
        </div>
        <div class="mb-1"><span class="fw-bold">Dated:</span> 16-12-2025</div>
      </div>
    </div>

    <!-- Source Table -->
    <div class="text-center py-1 fw-bold">Source (Consumption)</div>
    <table
      class="table table-bordered border-dark mb-0 text-center"
      style="font-size: 0.9rem;"
    >
      <thead class="table-light">
        <tr>
          <th style="width: 50px;">S.No.</th>
          <th class="text-start">Description of Goods</th>
          <th style="width: 150px;">Warehouse</th>
          <th style="width: 100px;">Batch</th>
          <th style="width: 100px;">Quantity</th>
          <th style="width: 100px;">Rate</th>
          <th style="width: 150px;">Amount</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td class="text-start">Deep Kadhai 07 (2mm)</td>
          <td>Packing</td>
          <td></td>
          <td>200.00 pc</td>
          <td>15.00</td>
          <td class="text-end">3,000.00</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="4" class="text-end fw-bold">Total</td>
          <td class="fw-bold">200.00</td>
          <td></td>
          <td class="text-end fw-bold">3,000.00</td>
        </tr>
      </tfoot>
    </table>

    <!-- Destination Table -->
    <div class="text-center py-1 fw-bold border-top border-dark">
      Destination (Production)
    </div>
    <table
      class="table table-bordered border-dark mb-0 text-center"
      style="font-size: 0.9rem;"
    >
      <thead class="table-light">
        <tr>
          <th style="width: 50px;">S.No.</th>
          <th class="text-start">Description of Goods</th>
          <th style="width: 150px;">Warehouse</th>
          <th style="width: 100px;">Batch</th>
          <th style="width: 100px;">Quantity</th>
          <th style="width: 100px;">Rate</th>
          <th style="width: 150px;">Amount</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td class="text-start">Deep Kadhai 07 (2mm)</td>
          <td>Main Location</td>
          <td></td>
          <td>200.00 pc</td>
          <td>15.00</td>
          <td class="text-end">3,000.00</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="4" class="text-end fw-bold">Total</td>
          <td class="fw-bold">200.00</td>
          <td></td>
          <td class="text-end fw-bold">3,000.00</td>
        </tr>
      </tfoot>
    </table>
  </div>

  <!-- Footer Info -->
  <div class="mt-4">
    <div class="mb-3">
      <div class="fst-italic fw-medium">Remarks:</div>
      <div class="fst-italic">dswcaswxaxaxa</div>
    </div>

    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR Three Thousand Only
    </p>

    <div class="row mt-5">
      <div class="col-8">
        <p class="mb-1 fw-bold">Account Number : 235605001136</p>
        <p class="mb-1 fw-bold">Bank : ICICI Bank</p>
        <p class="mb-1 fw-bold">IFSC CODE : ICIC0002356</p>

        <div class="mt-4 small">
          <p class="mb-1">1. Goods once sold will not be taken back.</p>
          <p class="mb-1">
            2. Interest @18% P.a. will be charged if the payment is not made
            with in the stipulated time.
          </p>
          <p class="mb-1">3. Subject to "Delhi" Jurisdiction only.</p>
        </div>
      </div>
      <div
        class="col-4 text-end d-flex flex-column justify-content-end align-items-end"
      >
        <div
          class="border border-secondary rounded-circle d-flex align-items-center justify-content-center mb-2"
          style="width: 100px; height: 100px; opacity: 0.5;"
        >
          <!-- Placeholder for Stamp/Signature -->
          <span
            class="small text-muted text-center"
            style="transform: rotate(-15deg);"
            >AKHIL STAINLESS<br />STEEL IND P. LTD</span
          >
        </div>
        <p class="fw-bold mb-0">Authorized Signatory</p>
      </div>
    </div>
  </div>
</div>

<style>
  .font-monospace {
    font-family: "Courier New", Courier, monospace !important;
  }
  .table-bordered > :not(caption) > * > * {
    border-width: 1px;
  }
  .border {
    border-width: 1.5px !important;
  }
</style>
