<script>
  // Transaction View: Delivery Challan
  // Layout based on deliveryChalan/delivery chalan.png
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

  <h5 class="text-center fw-bold text-decoration-underline mb-3">
    Delivery Challan
  </h5>

  <!-- Details Box -->
  <div class="border border-dark mb-0">
    <div class="row g-0">
      <!-- Left Column -->
      <div class="col-6 border-end border-dark p-2">
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 140px;"
            >Delivery Challan No</span
          >
          <span>: DC2</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 140px;">Date</span>
          <span>: 16-12-2025</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 140px;"
            >Purchase Order No</span
          >
          <span>: 12</span>
        </div>
      </div>
      <!-- Right Column -->
      <div class="col-6 p-2">
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">Transport</span>
          <span>: dwdxwx</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">Vehicle No.</span>
          <span>: asxax</span>
        </div>
        <div class="d-flex mb-1">
          <span class="fw-bold me-2" style="width: 100px;">GR/RR No.</span>
          <span>: asxaxax</span>
        </div>
      </div>
    </div>

    <!-- Parties -->
    <div class="row g-0 border-top border-dark">
      <!-- Billed To -->
      <div class="col-6 border-end border-dark">
        <div
          class="fw-bold text-center border-bottom border-dark py-1 bg-light"
        >
          Details of Receiver (Billed To)
        </div>
        <div class="p-2">
          <div class="fw-bold">MAGNUM MACHINES & TOOLS</div>
          <div>
            191, First Floor, Khasra No. 31/23, Matiyala Extension, Behind DPS,
            Sector 3, Dwarka, New Delhi
          </div>
          <div>Delhi-110059</div>
          <div><span class="fw-bold">GSTIN:</span> 07ABOFM1262D1ZE</div>
          <div><span class="fw-bold">Place Of Supply:</span> 07-Delhi</div>
        </div>
      </div>
      <!-- Shipped To -->
      <div class="col-6">
        <div
          class="fw-bold text-center border-bottom border-dark py-1 bg-light"
        >
          Details of Consignee (Shipped To)
        </div>
        <div class="p-2">
          <div class="fw-bold">MAGNUM MACHINES & TOOLS</div>
          <div>
            191, First Floor, Khasra No. 31/23, Matiyala Extension, Behind DPS,
            Sector 3, Dwarka, New Delhi
          </div>
          <div>Delhi-110059</div>
          <div><span class="fw-bold">GSTIN:</span> 07ABOFM1262D1ZE</div>
          <div><span class="fw-bold">Place Of Supply:</span> 07-Delhi</div>
        </div>
      </div>
    </div>

    <!-- Item Table -->
    <div class="border-top border-dark">
      <table
        class="table table-bordered border-dark mb-0 text-center"
        style="font-size: 0.9rem;"
      >
        <thead class="table-light">
          <tr>
            <th style="width: 40px;">#</th>
            <th class="text-start">Description</th>
            <th style="width: 60px;">HSN</th>
            <th style="width: 80px;">QTY</th>
            <th style="width: 60px;">Units</th>
            <th style="width: 90px;">Rate</th>
            <th style="width: 60px;">Per</th>
            <th style="width: 120px;">Amount</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td class="text-start">
              <div class="fw-bold">Deep Kadhai 07 (2mm)</div>
            </td>
            <td>7323</td>
            <td>20.00</td>
            <td>pc</td>
            <td>345.00</td>
            <td>pc</td>
            <td class="text-end">6,900.00</td>
          </tr>
          <!-- Empty rows/spacing -->
          <tr style="height: 100px;">
            <td colspan="8"></td>
          </tr>
        </tbody>
        <tfoot class="border-top border-dark">
          <tr>
            <td colspan="7" class="text-end fw-bold">Subtotal</td>
            <td class="text-end fw-bold">6,900.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Discount On Sale</td>
            <td class="text-end fw-bold">(690.00)</td>
          </tr>
          <tr>
            <td colspan="8" class="border-bottom-0 p-0"
              ><hr class="my-0 border-dark" /></td
            >
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Amount (Tax Exclusive)</td>
            <td class="text-end fw-bold">6,210.00</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">GST@5%</td>
            <td class="text-end fw-bold">310.50</td>
          </tr>
          <tr>
            <td colspan="7" class="text-end fw-bold">Round Off</td>
            <td class="text-end fw-bold">0.50</td>
          </tr>
          <tr>
            <td colspan="3" class="text-start fw-bold border-end-0">Total</td>
            <td class="fw-bold border-start-0 border-end-0">20.00</td>
            <td colspan="3" class="border-start-0"></td>
            <td class="text-end fw-bold">INR 6,521.00</td>
          </tr>
        </tfoot>
      </table>
    </div>
  </div>

  <!-- Footer Info -->
  <div class="mt-2">
    <p class="mb-1">
      <span class="fw-bold">Amount (in words) :</span> INR Six Thousand Five Hundred
      Twenty One Only
    </p>
    <p class="mb-4"><span class="fw-bold">Total Tax:</span> 310.50</p>

    <div class="row mt-5">
      <div class="col-8 d-flex flex-column justify-content-end">
        <p class="mb-0 fw-bold">Received in Good Condition</p>
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

    <div class="text-center mt-5 small text-muted">
      This is computer generated invoice
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
  .small {
    font-size: 0.85rem;
  }
</style>
