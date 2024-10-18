<template>
    <div class="flex gap-2 justify-between bg-white p-4 border rounded-lg shadow">
        <div class="col-span-2" role="form" aria-label="Formulário para criação de uma nova tarefa">
            <label for="task" class="block text-sm font-medium leading-6 text-gray-900">Tarefa</label>
            <div class="relative mt-2 rounded-md shadow-sm">
                <input type="text" name="task" id="task"
                    class="block w-full rounded-md border-0 py-1.5 pl-7 pr-20 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
                    placeholder="Nome da tarefa" />
            </div>
        </div>

        <div class="flex items-center justify-between gap-2">
            <section>
                <strong>00:00:00</strong>
            </section>
            <button>
                <Play />
                Play
            </button>
            <button>
                <Pause />
                Pause
            </button>
        </div>
    </div>
</template>

<script setup lang="ts">
    import { Play, Pause } from 'lucide-vue-next'; 
</script>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: "Forms"
    });
</script>