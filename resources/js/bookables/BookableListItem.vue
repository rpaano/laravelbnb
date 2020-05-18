<template>
    <div class="card w-100">
        <div class="card-body">
            <div class="card-title">
                <h5>{{ title }}</h5>
                <div class="card-text">
                    <p>{{ description }}</p>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        props: {
            'title': String,
            'description': String,
            'id': Number
        },
    }
</script>
