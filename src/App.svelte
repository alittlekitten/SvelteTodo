<script lang="ts">
import TailwindCSS from './TailwindCSS.svelte';

  let todos = [];
  let yes = false;
  const addTodo = () => {
    todos = [...todos, ''];
  }
  const removeTodo = (index) => {
    todos = [...todos.slice(0, index), ...todos.slice(index+1)];
  }
</script>

<main>
  <div class="flex flex-col justify-center items-center">
      <p class="text-5xl font-bold my-5 font-body "><span class="underline decoration-red-500">Svelte</span> & <span class="underline decoration-yellow-500">Vite</span> & <span class="underline decoration-sky-500">TailwindCSS</span> TodoList</p>
      {#each todos as todo, index}
        <div class="flex flex-row items-center m-5">
          <input class="bg-white shadow-lg rounded h-6 w-6" type="checkbox" />
          <input class="bg-white shadow-lg rounded px-6 pt-6 pb-6 h-4 ml-5" bind:value={todos[index]} />
          <button class="bg-red-500 shadow-lg hover:bg-red-700 text-white font-bold py-2 px-4 ml-5 rounded" on:click={()=>removeTodo(index)}>X</button>
          <br>
        </div>
      {/each}
    

    <button class="bg-blue-500 shadow-lg hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" on:click={addTodo}>추가</button>
  </div>
</main>

<TailwindCSS />