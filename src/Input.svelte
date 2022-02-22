<script>
    export let placeholder;
    export let type;
</script>

<div>
    <input type={type} placeholder={placeholder} class="input"/>
</div>

<style>
    .input{
        border-radius: 7px;
        height: 40px;
        width: 100%;
    }
</style>