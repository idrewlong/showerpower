<script>
        import { onMount } from 'svelte';
      
      let counters = 0;
      const targetValues = 10
      
      
      function incrementCounter(index) {
        if (counters[index] < targetValues[index]) {
          counters[index] += 1;
      
          setTimeout(() => incrementCounter(index), 0.1);
        }
      }
      
      
      onMount(() => {
      
        for (let i = 0; i < counters.length; i++) {
          incrementCounter(i);
        }
      });
      </script>