<template>
    <div>
        <div class="title">
            <div class="quote-box">
                <slot name="quotetitle">
                </slot>
            </div>
        </div>

        <div class="quote-box">
            <slot name="quotedesc"></slot>
            <slot></slot>
        </div>
    </div>
    
</template>
<script>
export default {
  data() {
    return {
    
    };
  }
};
</script>
<style scoped>
.quote-box {
  border: 1px solid #ccc;
  box-shadow: 2px 2px 2px #ccc;
  padding: 10px auto;
  text-align: center;
  margin-bottom: 20px;
}

.title {font-style: italic}

h2 {
  color: Red;
  font-size: 30px;
}
</style>