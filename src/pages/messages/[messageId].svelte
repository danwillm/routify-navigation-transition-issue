<script>
    import {params} from '@roxi/routify';
    import {fade} from "svelte/transition";
</script>
<div transition:fade>
    <p>Message {$params.messageId}</p>
</div>
