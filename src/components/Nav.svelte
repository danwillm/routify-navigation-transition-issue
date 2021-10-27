<script>
    import {goto, metatags} from '@roxi/routify';

    let enabled = true;
</script>
<div class="flex flex-no-wrap">
    <div style="min-height: 716px" class="w-64 absolute sm:relative bg-gray-800 shadow md:h-full flex-col justify-between hidden sm:flex">
        <div class="px-8">
            <div class="h-16 w-full flex items-center">
            </div>
            <ul class="mt-12">
                {#if enabled}
                    <li class="flex w-full justify-between text-gray-400 cursor-pointer items-center mb-6">
                        <a on:click={() => $goto('/')} class="flex items-center focus:outline-none focus:ring-2 focus:ring-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-grid" width="18" height="18" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                <rect x="4" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="4" y="14" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="14" width="6" height="6" rx="1"></rect>
                            </svg>
                            <span class="text-sm ml-2">Dashboard</span>
                        </a>
                    </li>
                    <li class="flex w-full justify-between text-gray-400 cursor-pointer items-center mb-6">
                        <a on:click={() => $goto('/messages')} class="flex items-center focus:outline-none focus:ring-2 focus:ring-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-grid" width="18" height="18" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                <rect x="4" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="4" y="14" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="14" width="6" height="6" rx="1"></rect>
                            </svg>
                            <span class="text-sm ml-2">Go to messages</span>
                        </a>
                    </li>
                    <li class="flex w-full justify-between text-gray-400 hover:text-gray-300 cursor-pointer items-center mb-6">
                        <a on:click={() => $goto('/anotherpage')} class="flex items-center focus:outline-none focus:ring-2 focus:ring-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-puzzle" width="18" height="18" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                <path d="M4 7h3a1 1 0 0 0 1 -1v-1a2 2 0 0 1 4 0v1a1 1 0 0 0 1 1h3a1 1 0 0 1 1 1v3a1 1 0 0 0 1 1h1a2 2 0 0 1 0 4h-1a1 1 0 0 0 -1 1v3a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-1a2 2 0 0 0 -4 0v1a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1h1a2 2 0 0 0 0 -4h-1a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1"></path>
                            </svg>
                            <span class="text-sm ml-2">Another page</span>
                        </a>
                    </li>
                    {/if}
            </ul>
        </div>
    </div>
</div>