<script>
  // Spreadsheet visual
</script>

<div class="absolute inset-0 bg-gray-100 flex items-center justify-center overflow-hidden">
  <div class="w-full h-full p-8 flex items-center justify-center">
    <div class="bg-white rounded-lg shadow-lg w-full h-full overflow-hidden border border-gray-200 text-[10px]">
       <!-- Fake spreadsheet header -->
       <div class="flex border-b border-gray-200 bg-gray-50">
         <div class="w-8 border-r border-gray-200 p-1 text-center text-gray-400">#</div>
         <div class="flex-1 p-1 border-r border-gray-200 font-medium text-gray-600">Company Name</div>
         <div class="flex-1 p-1 border-r border-gray-200 font-medium text-gray-600">Industry</div>
         <div class="flex-1 p-1 border-r border-gray-200 font-medium text-gray-600">Status</div>
         <div class="flex-1 p-1 border-r border-gray-200 font-medium text-gray-600">Revenue</div>
       </div>
       <!-- Rows -->
       {#each Array(15) as _, i}
         <div class="flex border-b border-gray-100 hover:bg-blue-50/50">
           <div class="w-8 border-r border-gray-100 p-1 text-center text-gray-400 bg-gray-50">{i + 1}</div>
           <div class="flex-1 p-1 border-r border-gray-100 text-gray-800">Acme Corp {i}</div>
           <div class="flex-1 p-1 border-r border-gray-100 text-gray-600">Technology</div>
           <div class="flex-1 p-1 border-r border-gray-100">
             <span class="px-1.5 py-0.5 rounded-full bg-green-100 text-green-700 text-[8px]">Active</span>
           </div>
           <div class="flex-1 p-1 border-r border-gray-100 text-gray-600">$10M - $50M</div>
         </div>
       {/each}
    </div>
  </div>
</div>
