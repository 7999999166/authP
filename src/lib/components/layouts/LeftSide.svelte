<script>
let {children} = $props();
  
</script>

<div class="container-fluid">  
    <div class="row">
        <div class="col-12 theme-pallate-nav g-0" style:height={"100px"}>
            <div class="d-flex flex-row h-100">
                <div style:width={"250px"}>
                    <div class="d-flex align-items-center justify-content-center h-100 p-2">
                        <img src="/logo.png" alt="" class="logo-img">
                    </div>
                </div>
                <div class="flex-fill" style:align-content={"center"}>
                    <div class="d-flex flex-column justify-content-center p-2">
                        <h5 class="text-center h-75 pb-1 company-name">Company Name</h5>
                        <div class="btn-group" role="group" aria-label="Default button group">
                            <button type="button" class="btn theme-nav-btn">Dashboard</button>
                            <button type="button" class="btn theme-nav-btn">Masters</button>
                            <button type="button" class="btn theme-nav-btn">Transactions</button>
                            <button type="button" class="btn theme-nav-btn">Reports</button>
                            <button type="button" class="btn theme-nav-btn">AI Assistant</button>
                            <button type="button" class="btn theme-nav-btn">Settings</button>
                        </div>
                    </div>
                </div>
                <div class="ms-auto" style:width={"250px"} style:align-content={"center"}>
                    <div class="d-flex flex-row justify-content-center gap-3 p-3">
                        <div class="d-flex flex-column align-items-center icon-container">
                            <i class="bi bi-arrow-clockwise theme-icon"></i>
                            <span class="icon-label">Refresh</span>
                        </div>
                        <div class="d-flex flex-column align-items-center icon-container">
                            <i class="bi bi-arrow-repeat theme-icon"></i>
                            <span class="icon-label">Sync</span>
                        </div>
                        <div class="d-flex flex-column align-items-center icon-container">
                            <i class="bi bi-bell-fill theme-icon"></i>
                            <span class="icon-label">Notifications</span>
                        </div>
                        <div class="d-flex flex-column align-items-center icon-container">
                            <i class="bi bi-person-circle theme-icon"></i>
                            <span class="icon-label">Profile</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-12 g-0 overflow-hidden content">
            <div class="d-flex flex-row h-100"> 
                <div class="h-100 theme-pallate-side" style:min-width={"250px"}></div>
                <div class="flex-fill ms-auto h-100 theme-pallate-content">
                   {@render children()}
                </div>
            </div>
        </div>
    </div>
</div>

<style>

 .content {
  height: calc(100vh - 100px);
} 

.theme-pallate-content{
   background-color: #e3f2fd;
}

.theme-pallate-side{
    background-color: #1565c0
}

.theme-pallate-nav{
  background-color: #0d47a1; 
  border-bottom: solid .5px #e3f2fd ; 
}
::-webkit-scrollbar{
    display: none;
}

.theme-icon {
    color: #e3f2fd;
    font-size: 1.4rem;
    cursor: pointer;
    transition: transform 0.2s;
}

.theme-icon:hover {
    transform: scale(1.1);
}

.icon-label {
    color: #e3f2fd;
    font-size: 0.75rem;
    margin-top: 0.25rem;
}

.icon-container {
    cursor: pointer;
}

.logo-img {
    max-height: 170px;
    max-width: 230px;
    width: 100%;
    height: auto;
    object-fit: contain;
}

.company-name {
    color: #e3f2fd;
    font-weight: 600;
    letter-spacing: 0.5px;
}

.theme-nav-btn {
    color: #e3f2fd;
    border-color: #e3f2fd;
    background-color: transparent;
    transition: all 0.2s;
}

.theme-nav-btn:hover {
    background-color: #1565c0;
    border-color: #e3f2fd;
    color: #e3f2fd;
}

.theme-nav-btn:active,
.theme-nav-btn.active {
    background-color: #1565c0;
    border-color: #e3f2fd;
    color: #e3f2fd;
}
   
</style>