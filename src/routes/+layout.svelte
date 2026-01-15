<script>
  import { page } from "$app/stores";
  import { onMount } from "svelte";
  import "../app.css";
  import RightSide from "$lib/components/layouts/RightSide.svelte";
  import LeftSide from "$lib/components/layouts/LeftSide.svelte";
  import MasterLayout from "$lib/components/layouts/MasterLayout.svelte";
  import NoSide from "$lib/components/layouts/NoSide.svelte";

  let folderName = $derived($page.url.pathname.split("/").filter(Boolean)[0] );
  let routeName =  $derived($page.url.pathname.split("/").filter(Boolean).pop() );
  let { children } = $props();

  onMount(() => {
    setTimeout(() => {
      if (window.bootstrap) {
        const popoverTriggerList = document.querySelectorAll('[data-bs-toggle="popover"]');
        [...popoverTriggerList].forEach(popoverTriggerEl => {
          const popover = new window.bootstrap.Popover(popoverTriggerEl, {
            container: 'body',
            sanitize: false,
            fallbackPlacements: [],
            customClass: 'custom-popover',
            popperConfig: {
              modifiers: [
                {
                  name: 'offset',
                  options: {
                    offset: [40, 25]
                  }
                },
                {
                  name: 'arrow',
                  options: {
                    element: '.popover-arrow'
                  }
                },
                {
                  name: 'flip',
                  enabled: false
                },
                {
                  name: 'preventOverflow',
                  options: {
                    altAxis: true,
                    padding: 8
                  }
                }
              ]
            }
          });
          
          popoverTriggerEl.addEventListener('click', function(e) {
            e.stopPropagation();
            document.querySelectorAll('[data-bs-toggle="popover"]').forEach(el => {
              if (el !== popoverTriggerEl) {
                const otherPopover = window.bootstrap.Popover.getInstance(el);
                if (otherPopover) otherPopover.hide();
              }
            });
          });
        });
        
        document.addEventListener('click', function(e) {
          if (!e.target.closest('[data-bs-toggle="popover"]') && !e.target.closest('.popover')) {
            document.querySelectorAll('[data-bs-toggle="popover"]').forEach(el => {
              const popover = window.bootstrap.Popover.getInstance(el);
              if (popover) popover.hide();
            });
          }
        });

        const scrollContainers = document.querySelectorAll('.sidebar-scroll');
        scrollContainers.forEach(container => {
          container.addEventListener('scroll', function() {
            document.querySelectorAll('[data-bs-toggle="popover"]').forEach(el => {
              const popover = window.bootstrap.Popover.getInstance(el);
              if (popover) popover.hide();
            });
          });
        });
      } else {
        console.error('Bootstrap not loaded');
      }
    }, 100);
  });
</script>

<svelte:head>
  <script src="/bootstrap.bundle.min.js"></script>
  <script src="/axios.min.js"></script>
</svelte:head>
<div class="app">
  {#if routeName === "zone"}
  <RightSide {onlyRightSide}>{@render children()}</RightSide>  
  {:else if routeName === "done"}
  <LeftSide>{@render children()}</LeftSide>  
  {:else if folderName === "masterCreate"}
  <MasterLayout {masterMenu} {ledgerMenu}>{@render children()}</MasterLayout> 
  {:else}
  <NoSide>{@render children()}</NoSide>
  {/if}
</div>

{#snippet onlyRightSide()}
  <div>
    <h1>Hello Kanik</h1>
    <p>How Are You</p>
  </div>
{/snippet}

{#snippet masterMenu()}
  <div class="overflow-y-scroll" style:height="100%">
  <ul class="list-group master-menu-list mb-3">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
</ul>
  </div>
{/snippet}

{#snippet ledgerMenu()}
 <div class="accordion" id="accordionExample">
  <div class="accordion-item ">
    <h2 class="accordion-header">
      <button class="accordion-button " type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        Accordion Item 1
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
      <div class="accordion-body">
          <ul class="list-group master-menu-list">
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">View Ledger</a><a href="#" class="popover-menu-item">Edit</a><a href="#" class="popover-menu-item">Delete</a></div>'>First item</span>
   </li>

    <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
   
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        Accordion Item 2
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">And a fifth one</li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item 3
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item 4
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item 5
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item 6
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
</ul>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Accordion Item 7
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
           <ul class="list-group master-menu-list">
   <li class="list-group-item">An item</li>
   <li class="list-group-item">A second item</li>
   <li class="list-group-item">A third item</li>
   <li class="list-group-item">A fourth item</li>
   <li class="list-group-item">
      <span type="button" data-bs-toggle="popover" data-bs-placement="left" data-bs-trigger="click" data-bs-html="true" data-bs-content='<div class="popover-custom-menu"><a href="#" class="popover-menu-item">An item</a><a href="#" class="popover-menu-item">A second item</a><a href="#" class="popover-menu-item">A third item</a><a href="#" class="popover-menu-item">A fourth item</a><a href="#" class="popover-menu-item">And a fifth one</a></div>'>Second item</span>
   </li>
</ul>
      </div>
    </div>
  </div>
</div>
{/snippet}

<style>

::-webkit-scrollbar {
    width: 0px;
}

.master-menu-list .list-group-item {
  background-color: transparent;
  border-color: rgba(255, 255, 255, 0.2);
  color: white;
}

.accordion .accordion-item {
  background-color: transparent;
  border-color: rgba(255, 255, 255, 0.2);
}

.accordion .accordion-button {
  background-color: transparent;
  color: white;
  border-color: rgba(255, 255, 255, 0.2);
}

.accordion .accordion-button:not(.collapsed) {
  background-color: rgba(255, 255, 255, 0.1);
  color: white;
}

.accordion .accordion-body {
  background-color: transparent;
  color: white;
}

:global(.popover),
:global(.custom-popover) {
  --bs-popover-max-width: 250px;
  --bs-popover-bg: rgba(21, 101, 192, 0.95);
  --bs-popover-border-color: rgba(255, 255, 255, 0.2);
  min-width: 180px;
  background-color: rgba(21, 101, 192, 0.95) !important;
  border: 1px solid rgba(255, 255, 255, 0.2) !important;
}

:global(.popover .popover-arrow::before),
:global(.custom-popover .popover-arrow::before) {
  border-left-color: rgba(255, 255, 255, 0.2) !important;
}

:global(.popover .popover-arrow::after),
:global(.custom-popover .popover-arrow::after) {
  border-left-color: rgba(21, 101, 192, 0.95) !important;
}

:global(.popover-body) {
  padding: 0.5rem 0;
}

:global(.popover-custom-menu) {
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}

:global(.popover-menu-item) {
  padding: 0.6rem .8rem;
  color: white;
  text-decoration: none;
  background-color: transparent;
  border: none;
  display: block;
  transition: background-color 0.2s;
  font-size: 0.9rem;
}

:global(.popover-menu-item:hover) {
  background-color: rgba(255, 255, 255, 0.1);
  color: white;
}
</style>
