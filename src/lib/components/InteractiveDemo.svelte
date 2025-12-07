<section class="py-24 px-6 bg-gray-50">
  <div class="max-w-7xl mx-auto">
    <div class="mb-12">
      <h2 class="text-3xl md:text-4xl font-medium text-gray-900 mb-2">Before you book a demo</h2>
      <p class="text-3xl md:text-4xl font-medium text-gray-400">Explore our product</p>
    </div>

    <!-- Demo UI Container -->
    <div class="bg-white rounded-xl shadow-xl border border-gray-200 overflow-hidden">
      <!-- Top Bar -->
      <div class="border-b border-gray-200 flex items-center px-4 py-2 gap-4 text-xs font-medium text-gray-600">
        <div class="flex items-center gap-1 px-2 py-1 bg-gray-100 rounded cursor-pointer">
          <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/></svg>
          AI Agents
        </div>
        <div class="flex items-center gap-1 px-2 py-1 hover:bg-gray-50 rounded cursor-pointer">
          <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/></svg>
          Knowledge
        </div>
        <div class="flex items-center gap-1 px-2 py-1 hover:bg-gray-50 rounded cursor-pointer">
          <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/></svg>
          Doc Gen
        </div>
      </div>

      <!-- Toolbar -->
      <div class="border-b border-gray-200 p-4 flex items-start justify-between bg-gray-50/50">
        <div class="flex gap-8 text-xs">
          <div class="space-y-1">
            <div class="text-gray-500">Input files, pick agent, or let</div>
            <div class="text-gray-900 font-medium">Concierge pick one for you</div>
          </div>
          <div class="space-y-1">
            <div class="text-gray-900 font-medium flex items-center gap-1">
              An AI generated table starts building
              <span class="w-2 h-0.5 bg-black"></span>
            </div>
          </div>
          <div class="space-y-1">
            <div class="text-gray-500">Configure each step in further</div>
            <div class="text-gray-500">properties</div>
          </div>
          <div class="space-y-1">
            <div class="text-gray-500">Iterate and improve your agent as</div>
            <div class="text-gray-500">you like</div>
          </div>
          <div class="space-y-1">
            <div class="text-gray-500">Zoom in on doc level and iterate</div>
            <div class="text-gray-500">any detail</div>
          </div>
        </div>
      </div>

      <!-- Main Interface -->
      <div class="h-[600px] bg-white relative flex flex-col">
        <!-- Breadcrumbs & Actions -->
        <div class="border-b border-gray-200 px-4 py-2 flex items-center justify-between text-xs">
           <div class="flex items-center gap-2 text-gray-500">
             <span>Home</span>
             <span>/</span>
             <span class="text-gray-900 font-medium">Agent name</span>
           </div>
           <div class="flex items-center gap-2">
             <div class="flex bg-gray-100 rounded p-0.5">
               <button class="px-3 py-1 bg-white rounded shadow-sm text-gray-900 font-medium">Build</button>
               <button class="px-3 py-1 text-gray-500">Review</button>
               <button class="px-3 py-1 text-gray-500">Workflow</button>
             </div>
             <div class="h-4 w-px bg-gray-200 mx-2"></div>
             <button class="text-gray-500">Export</button>
             <button class="bg-black text-white px-3 py-1 rounded">Share</button>
           </div>
        </div>

        <!-- Table Header -->
        <div class="border-b border-gray-200 flex text-xs font-medium text-gray-500 bg-gray-50">
          <div class="w-10 p-2 border-r border-gray-200 text-center">
            <input type="checkbox" class="rounded border-gray-300" />
          </div>
          <div class="w-10 p-2 border-r border-gray-200 text-center">#</div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/></svg>
            File Input
          </div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/></svg>
            Clauses
          </div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/></svg>
            State
          </div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/></svg>
            Reference
          </div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 21h18M5 21V7l8-4 8 4v14"/></svg>
            Company
          </div>
          <div class="flex-1 p-2 border-r border-gray-200 flex items-center gap-1">
            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
            Financials
          </div>
        </div>

        <!-- Empty State / Rows -->
        <div class="flex-1 bg-white">
          <div class="flex border-b border-gray-100 h-10">
            <div class="w-10 border-r border-gray-100 bg-gray-50 text-center py-3 text-xs text-gray-400">1</div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
          </div>
          <div class="flex border-b border-gray-100 h-10">
            <div class="w-10 border-r border-gray-100 bg-gray-50 text-center py-3 text-xs text-gray-400">2</div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
            <div class="flex-1 border-r border-gray-100"></div>
          </div>
        </div>

        <!-- Floating Action Button -->
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 bg-gray-900/90 backdrop-blur text-white px-6 py-3 rounded-full shadow-2xl flex items-center gap-4 hover:bg-black transition-colors cursor-pointer group">
          <div class="text-left">
            <div class="font-medium">Agent Tables</div>
            <div class="text-xs text-gray-400">Purpose-built for specialized tasks.</div>
          </div>
          <div class="bg-white/10 px-3 py-1 rounded-full text-xs font-medium group-hover:bg-white/20 transition-colors">Explore</div>
        </div>

      </div>
    </div>
  </div>
</section>
