<script>
    import { onMount } from 'svelte';
    import "../app.css";
  
    let blob;
    
  
    onMount(() => {
      /* -- Glow effect -- */
      window.onpointermove = event => { 
        const { clientX, clientY } = event;
          
        blob.animate({
          left: `${clientX}px`,
          top: `${clientY}px`
        }, { duration: 3000, fill: "forwards" });
      }
    });
</script>
  


<div id="blob" bind:this={blob}></div>
    <div id="blur"></div>


<style>
    @keyframes rotate {
        from {
            rotate: 0deg;
        }
        
        50% {
            scale: 1 1.5;
        }
        
        to {
            rotate: 360deg;
        }
    }

    #blob {
        background-color: white;
        height: 26vmax;
        aspect-ratio: 1;
        position: absolute;
        left: 50%;
        top: 50%;
        translate: -50% -50%;
        border-radius: 50%;
        background: linear-gradient(to right, rgb(255, 206, 127), rgb(242, 167, 46));
        animation: rotate 20s infinite;
        opacity: 0.9;
        overflow: hidden;
    }

    #blur {
        height: 100%;
        width: 100%;
        position: absolute;
        z-index: 2;
        backdrop-filter: blur(12vmax);
        overflow: hidden;
    }
</style>
