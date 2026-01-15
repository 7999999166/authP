<script>
  // Transaction View: Deposit Cash
  // Layout based on Standard Voucher (Similar to Contra)
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

  <!-- Voucher Box -->
  <div class="border border-dark mb-0">
    <!-- Title Row -->
    <div class="d-flex justify-content-end p-2 border-bottom border-dark">
      <div class="text-end">
        <h2 class="fw-bold mb-1">Deposit Cash</h2>
        <div class="mb-1"><span class="fw-bold">Voucher No.</span> DEP101</div>
        <div class="mb-1"><span class="fw-bold">Dated:</span> 12-12-2025</div>
      </div>
    </div>

    <!-- Table -->
    <table
      class="table table-bordered border-dark mb-0"
      style="font-size: 0.9rem;"
    >
      <thead class="table-light text-end">
        <tr>
          <th class="text-start border-bottom-dark">Particulars</th>
          <th style="width: 150px;" class="border-bottom-dark">Debit</th>
          <th style="width: 150px;" class="border-bottom-dark">Credit</th>
        </tr>
      </thead>
      <tbody>
        <tr style="height: 150px;">
          <td class="text-start align-top">
            <div class="fw-bold fst-italic mb-2">Deposited Into</div>
            <div class="mb-3 ms-3">ICICI BANK (235605001136)</div>
            <div class="fw-bold fst-italic mb-2">From</div>
            <div class="ms-3">Cash Account</div>
          </td>
          <td class="text-end align-top pt-5"> 15,000.00 </td>
          <td class="text-end align-bottom pb-3">
            <br /><br /><br />
            15,000.00
          </td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td class="fw-bold border-end-dark">Total</td>
          <td class="text-end fw-bold border-end-dark">INR 15,000.00</td>
          <td class="text-end fw-bold">INR 15,000.00</td>
        </tr>
      </tfoot>
    </table>
  </div>

  <!-- Footer -->
  <div class="row mt-5">
    <div class="col-8"></div>
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
