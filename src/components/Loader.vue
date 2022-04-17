<template>
    <div>
        <div class="page-loader">
            <div class="ring">
                <div></div><div></div><div></div><div></div>
            </div>
        </div>
    </div>
</template>

<script>
/* page loader */
window.addEventListener("load", function(){
    document.querySelector(".page-loader").classList.add("fade-out");
    
    this.setTimeout(function(){
    document.querySelector(".page-loader").style.display = "none";
    },600)
})
</script>