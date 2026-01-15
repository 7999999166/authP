<script>
  // Transaction View: Manufacturing Journal
  // Layout based on manufacturingJournal/manufacturing journal.png
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
        <h2 class="fw-bold mb-1">Manufacturing Journal</h2>
        <div class="mb-1">
          <span class="fw-bold">Manufacturing Journal No:</span> MFG2
        </div>
        <div class="mb-1"><span class="fw-bold">Dated:</span> 07-05-2025</div>
      </div>
    </div>

    <!-- Consumed Items Table -->
    <div class="text-center py-1 fw-bold">Consumed Items</div>
    <table
      class="table table-bordered border-dark mb-0 text-center"
      style="font-size: 0.9rem;"
    >
      <thead class="table-light">
        <tr>
          <th style="width: 50px;">S.No.</th>
          <th class="text-start">Description of Goods</th>
          <th style="width: 150px;">Quantity</th>
          <th style="width: 100px;">Rate</th>
          <th style="width: 150px;">Amount</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td class="text-start">Coil .50mm 49"</td>
          <td>1,500.00 kg</td>
          <td>150.00</td>
          <td class="text-end">2,25,000.00</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="4" class="text-end fw-bold">Cost of Components</td>
          <td class="text-end fw-bold">2,25,000.00</td>
        </tr>
        <tr>
          <td colspan="4" class="text-end fw-bold">Manufacturing Expense</td>
          <td class="text-end fw-bold">0.00</td>
        </tr>
        <tr>
          <td colspan="4" class="text-end fw-bold">Total</td>
          <td class="text-end fw-bold">2,25,000.00</td>
        </tr>
      </tfoot>
    </table>

    <!-- Manufactured Items Table -->
    <div class="text-center py-1 fw-bold border-top border-dark">
      Manufactured Items
    </div>
    <table
      class="table table-bordered border-dark mb-0 text-center"
      style="font-size: 0.9rem;"
    >
      <thead class="table-light">
        <tr>
          <th style="width: 50px;">S.No.</th>
          <th class="text-start">Description of Goods</th>
          <th style="width: 150px;">Quantity</th>
          <th style="width: 100px;">Rate</th>
          <th style="width: 120px;">% of Total Value</th>
          <th style="width: 150px;">Amount</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td class="text-start">SS CIRCLE 72202090</td>
          <td>1,300.00 kg</td>
          <td>154.04</td>
          <td>89.00</td>
          <td class="text-end">2,00,252.00</td>
        </tr>
        <tr>
          <td>2</td>
          <td class="text-start">Scrap</td>
          <td>26.00 kg</td>
          <td>951.92</td>
          <td>11.00</td>
          <td class="text-end">24,749.92</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td colspan="5" class="text-end fw-bold">Total</td>
          <td class="text-end fw-bold">2,25,000.00</td>
        </tr>
      </tfoot>
    </table>
  </div>

  <!-- Footer Info -->
  <div class="mt-4">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR Two Hundred Twenty Five
      Thousand Only
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
