<script>
  import Prep from '$lib/components/Prep.svelte';
  var discount = $state(false);
  var tax = $state(false);
  var otherCharges = $state(false);
  var dispatchDetails = $state(false);
  async function googleSignin() {

  await axios({
   method: 'get',
   url: 'https://strapijan-production.up.railway.app/api/connect/google',
   })
  .then( function (response) { console.log ( response.data.data )  });
 
  }
</script>

<div>
  <Prep name={"John"} />
  <button class="btn btn-primary ms-4" onclick={googleSignin}>Google Signin</button>
  <div class="row p-2">
    <div class="col-4 d-flex flex-column">
      <div class="form-check" style:height="40px" style:align-content="center">
        <input class="form-check-input" type="checkbox" bind:checked={discount} value="" id="checkDefault"/>
        <label class="form-check-label" for="checkDefault"> Discount </label>
      </div>
      <div class="form-check" style:height="40px" style:align-content="center">
        <input class="form-check-input" type="checkbox" bind:checked={tax} value="" id="checkDefault"/>
        <label class="form-check-label" for="checkDefault"> tax </label>
      </div>
      <div class="form-check" style:height="40px" style:align-content="center">
        <input class="form-check-input" type="checkbox" value="" id="checkDefault"/>
        <label class="form-check-label" for="checkDefault"> Other Charges </label>
      </div>
      <div class="form-check" style:height="40px" style:align-content="center">
        <input class="form-check-input" type="checkbox" value="" id="checkDefault"/>
        <label class="form-check-label" for="checkDefault"> Dispatch Details </label>
      </div>
    </div>
    <div class="col-4"></div>
    <div class="col-4">
      {#if discount }
      <div class="d-flex flex-row align-items-center justify-content-end" style:height="40px">
        <label for="exampleFormControlInput1" class="w-25 h-75" style:align-content="center">Sub Total</label>
        <input type="email" class="form-control w-50 h-75" id="exampleFormControlInput1" placeholder="0.00">
      </div>
      {/if}
      <div class={[tax? "visible" : "invisible","d-flex flex-row align-items-center justify-content-end "]} style:height="40px" style:align-content="center">
        <label for="exampleFormControlInput1" class="w-25 h-75" style:align-content="center">Tax Value</label>
        <input type="email" class="form-control w-50 h-75" id="exampleFormControlInput1" placeholder="0.00">
      </div>
      <div class="d-flex flex-row align-items-center justify-content-end" style:height="40px" style:align-content="center">
        <label for="exampleFormControlInput1" class="h-75 w-25" style:align-content="center" >Discount Amount</label>
        <input type="email" class="form-control w-50 h-75" id="exampleFormControlInput1" placeholder="0.00">
      </div>
      <div class="d-flex flex-row align-items-center justify-content-end" style:height="40px" style:align-content="center">
        <label for="exampleFormControlInput1" class="h-75 w-25" style:align-content="center">Total</label>
        <input type="email" class="form-control w-50 h-75" id="exampleFormControlInput1" placeholder="0.00">
      </div>
    </div>
  </div>
</div>

<style>
</style>
