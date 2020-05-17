<template>
    <div class="card">
        <div class="card-body">
            <div class="card-title">
                <h5>{{ itemTitle }}</h5>
                <div class="card-text">
                    <p>{{ itemDescription }}</p>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        props: {
            'itemTitle': String,
            'itemDescription': String,
            'price': Number
        },
    }
</script>
