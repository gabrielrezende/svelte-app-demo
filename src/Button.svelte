<script>
    export let width = "120px";
    export let fontColor = "#FFF";
    export let backgroundColor = "#ff8a00"
    export let onClick;
</script>

<div>
    <button
            class="button"
            style="width: {width}; color: {fontColor}; background-color:{backgroundColor}"
            on:click={()=>{onClick()}}
    >
        <slot></slot>
    </button>
</div>

<style>
    .button{
        border-radius: 7px;
        height: 40px;
        box-shadow: 2px 3px 3px #333;
        border: none;
        cursor: pointer;

    }

    .button:hover {
        filter: brightness(95%);
    }

</style>