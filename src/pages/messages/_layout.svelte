<script>
    import {goto, metatags} from '@roxi/routify';

    let messages = ['1', '2', '3'];
</script>
<div class="flex flex-no-wrap">
    <div style="min-height: 716px"
         class="w-64 absolute sm:relative bg-gray-800 shadow md:h-full flex-col justify-between hidden sm:flex">
        <div class="px-8">
            <div class="h-16 w-full flex items-center">
            </div>
            <ul class="mt-12">
                {#each messages as message}
                    <li class="flex w-full justify-between text-gray-400 cursor-pointer items-center mb-6">
                        <a on:click={() => $goto('./' + message)}
                           class="flex items-center focus:outline-none focus:ring-2 focus:ring-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-grid" width="18"
                                 height="18" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                 stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                <rect x="4" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="4" width="6" height="6" rx="1"></rect>
                                <rect x="4" y="14" width="6" height="6" rx="1"></rect>
                                <rect x="14" y="14" width="6" height="6" rx="1"></rect>
                            </svg>
                            <span class="text-sm ml-2">Message {message}</span>
                        </a>
                    </li>
                {/each}
            </ul>
        </div>
    </div>
    <div class="container mx-auto py-10 h-64 md:w-4/5 w-11/12 px-6">
        <div class="w-full h-full rounded border-dashed border-2 border-gray-300">
            <slot/>
        </div>
    </div>
</div>