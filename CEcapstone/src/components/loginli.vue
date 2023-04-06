<template>
    <div class="modal" v-if="show">
        <div class="modal-content">
            <span class="close" @click="closeModal">&times;</span>
            <slot></slot>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            show: false,
        };
    },
    methods: {
        openModal() {
            this.show = true;
        },
        closeModal() {
            this.show = false;
        },
    },
};
</script>
  
<style scoped>
.modal {
    display: none;
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgb(0, 0, 0);
    background-color: rgba(0, 0, 0, 0.4);
}

.modal-content {
    background-color: #fefefe;
    margin: 15% auto;
    padding: 20px;
    border: 1px solid #888;
    width: 80%;
}

.close {
    color: #aaa;
    float: right;
    font-size: 28px;
    font-weight: bold;
}

.close:hover,
.close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
}

form {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

label {
    font-size: 14px;
    font-weight: bold;
}

input {
    padding: 5px;
    border-radius: 5px;
    border: 1px solid #ddd;
}

button {
    background-color: #428bca;
    color: #fff;
    padding: 10px;
    border-radius: 5px;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #3071a9;
}
</style>