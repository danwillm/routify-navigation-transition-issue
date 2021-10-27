<script>
    import Nav from "../components/Nav.svelte";
    import { fade } from 'svelte/transition';
    import { BaseTransition } from '@roxi/routify/decorators'

    const configs = [
        {
            condition: (meta)=>true,
            transition: fade,
            /** inParams: {},  optional **/
            /** outParams: {}  optional **/
        }
    ]
</script>

<div class="flex flex-row">
    <Nav />
<!--    <BaseTransition {configs}>-->
<!--        <slot />-->
<!--    </BaseTransition>-->
    <slot />
</div>
