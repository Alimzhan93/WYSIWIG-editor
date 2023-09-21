<template>
  <div class="editor">
    <div class="toolbar">
      
      <button class="undo" @click="undo" type="button">
        <svg  xmlns="http://www.w3.org/2000/svg" width="42" height="38" viewBox="0 0 42 38" fill="none">
        <rect width="42" height="38" rx="4" fill="#282828"/>
        <path d="M28.6358 29.5824C28.3582 29.86 27.9929 30 27.6299 30C27.2645 30 26.8992 29.86 26.6216 29.5824C26.0664 29.0249 26.0664 28.1257 26.6216 27.5682C29.7604 24.4294 29.7604 19.3238 26.6216 16.1851C23.4852 13.0486 18.3772 13.0486 15.2408 16.1851L14.726 16.6999H18.1234C18.9087 16.6999 19.5469 17.3381 19.5469 18.1234C19.5469 18.911 18.9087 19.5469 18.1234 19.5469H11.4235C10.6382 19.5469 10 18.911 10 18.1234V11.4235C10 10.6382 10.6382 10 11.4235 10C12.2088 10 12.847 10.6382 12.847 11.4235V14.5528L13.2266 14.1732C17.4757 9.92408 24.3867 9.92408 28.6358 14.1732C32.8849 18.4223 32.8849 25.3333 28.6358 29.5824Z" fill="#639EFF"/>
      </svg>
      </button>
      
      <button class="redo" @click="redo" type="button">
        <svg  xmlns="http://www.w3.org/2000/svg" width="42" height="38" viewBox="0 0 42 38" fill="none">
          <rect width="42" height="38" rx="4" fill="#282828"/>
          <path d="M13.1868 29.5824C13.4644 29.86 13.8298 30 14.1928 30C14.5581 30 14.9235 29.86 15.2011 29.5824C15.7562 29.0249 15.7562 28.1257 15.2011 27.5682C12.0623 24.4294 12.0623 19.3238 15.2011 16.1851C18.3375 13.0486 23.4454 13.0486 26.5819 16.1851L27.0967 16.6999H23.6993C22.914 16.6999 22.2758 17.3381 22.2758 18.1234C22.2758 18.911 22.914 19.5469 23.6993 19.5469H30.3992C31.1845 19.5469 31.8227 18.911 31.8227 18.1234V11.4235C31.8227 10.6382 31.1845 10 30.3992 10C29.6139 10 28.9757 10.6382 28.9757 11.4235V14.5528L28.5961 14.1732C24.347 9.92408 17.4359 9.92408 13.1868 14.1732C8.93773 18.4223 8.93773 25.3333 13.1868 29.5824Z" fill="#639EFF"/>
      </svg>
      </button>
      
      <button class="formatHeader" @click="formatHeader">
        <svg  xmlns="http://www.w3.org/2000/svg" width="42" height="38" viewBox="0 0 42 38"  fill="none">
          <rect width="42" height="38" rx="4" fill="#282828"/>
          <path d="M24 4.5V7.0075C24 7.8375 23.3317 8.5075 22.5037 8.5075C21.6783 8.5075 21.0075 7.8375 21.0075 7.0075V6H15.4963V23H16.8454C17.6733 23 18.3416 23.6725 18.3416 24.5C18.3416 25.3275 17.6733 26 16.8454 26H11.1546C10.3267 26 9.65835 25.3275 9.65835 24.5C9.65835 23.6725 10.3267 23 11.1546 23H12.5037V6H6.99252V7.0075C6.99252 7.8375 6.3217 8.5075 5.49626 8.5075C4.66833 8.5075 4 7.8375 4 7.0075V4.5C4 3.6725 4.66833 3 5.49626 3H22.5037C23.3317 3 24 3.6725 24 4.5Z" fill="#639EFF"/>
        </svg>
      </button>
      
     
      <button class="formatParagraph" @click="formatParagraph">
        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 28 28" fill="none">
          <path d="M13.4876 9.74158V11.0604C13.4876 11.9872 12.7344 12.7404 11.8076 12.7404C11.004 12.7404 10.332 12.1748 10.1668 11.4216H9.0048V18.5868C9.8476 18.6792 10.5056 19.3932 10.5056 20.2584C10.5056 21.188 9.7524 21.9384 8.8256 21.9384H5.824C4.89439 21.9384 4.14399 21.188 4.14399 20.2584C4.14399 19.3932 4.7992 18.6792 5.64479 18.5868V11.4216H4.48C4.3148 12.1748 3.6428 12.7404 2.8392 12.7404C1.9124 12.7404 1.15919 11.9872 1.15919 11.0604V9.74158C1.15919 8.81198 1.9124 8.06158 2.8392 8.06158H11.8076C12.7344 8.06158 13.4876 8.81198 13.4876 9.74158Z" fill="#639EFF"/>
          <path d="M26.9192 9.74158V11.0604C26.9192 11.9872 26.1688 12.7404 25.2392 12.7404C24.4356 12.7404 23.7636 12.1748 23.5984 11.4216H22.4364V18.5868C23.2792 18.6792 23.9372 19.3932 23.9372 20.2584C23.9372 21.188 23.184 21.9384 22.2572 21.9384H19.2556C18.326 21.9384 17.5756 21.188 17.5756 20.2584C17.5756 19.3932 18.2308 18.6792 19.0764 18.5868V11.4216H17.9144C17.7492 12.1748 17.0772 12.7404 16.2708 12.7404C15.344 12.7404 14.5908 11.9872 14.5908 11.0604V9.74158C14.5908 8.81198 15.344 8.06158 16.2708 8.06158H25.2392C26.1688 8.06158 26.9192 8.81198 26.9192 9.74158Z" fill="#639EFF"/>
        </svg>
      </button>

      <button class="insertImage" @click="insertImage">
        <svg xmlns="http://www.w3.org/2000/svg" width="42" height="38" viewBox="0 0 42 38" fill="none">
          <rect x="4.57764e-05" width="42" height="38" rx="4" fill="#282828"/>
          <path d="M30.5652 9.07849H11.4348C10.6433 9.07849 10 9.72175 10 10.5133V27.4868C10 28.2783 10.6433 28.9215 11.4348 28.9215H30.5652C31.3567 28.9215 32 28.2783 32 27.4868V10.5133C32 9.72175 31.3567 9.07849 30.5652 9.07849ZM29.1304 26.052H12.8696V25.3274L15.9496 22.2474L17.3867 23.6822C17.9463 24.2441 18.855 24.2441 19.4146 23.6846L25.0843 18.0148L29.1304 22.0609V26.052ZM29.1304 18.0052L26.0983 14.9707C25.5363 14.4111 24.63 14.4111 24.068 14.9707L18.4007 20.6404L16.9635 19.2033C16.4039 18.6437 15.4952 18.6437 14.9357 19.2033L12.8696 21.2694V11.9481H29.1304V18.0052Z" fill="#639EFF"/>
          <path d="M17.7591 17.2558C16.765 17.2558 15.9563 16.447 15.9563 15.453C15.9563 14.4589 16.765 13.6502 17.7591 13.6502C18.7531 13.6502 19.5619 14.4589 19.5619 15.453C19.5619 16.447 18.7531 17.2558 17.7591 17.2558Z" fill="#639EFF"/>
        </svg>
      </button>
      <button class="copyHTML" @click="copyHTML">Скопировать HTML</button>
    </div>
    <div
      class="content"
      ref="editor" contenteditable="true" @input="updateContent"
    ></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      content: '',
    };
  },
  methods: {
    undo() {
      document.execCommand('undo');
    },
    redo() {
      document.execCommand('redo');
    },
    formatHeader() {
      document.execCommand('formatBlock', false, 'h1');
    },
    formatParagraph() {
      document.execCommand('formatBlock', false, 'p');
    },
    insertImage() {
      const url = prompt('Введите URL картинки:');
      if (url) {
        document.execCommand('insertImage', false, url);
      }
    },
    copyHTML() {
      const editorContent = this.$refs.editor.innerHTML;
      const tempTextarea = document.createElement('textarea');
      tempTextarea.value = editorContent;
      document.body.appendChild(tempTextarea);
      tempTextarea.select();
      document.execCommand('copy');
      document.body.removeChild(tempTextarea);
      alert('HTML скопирован в буфер обмена.');
    },
    updateContent() {
      this.content = this.$refs.editor.innerHTML;
    },
  },
};


</script>

<style scoped>
.editor {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
.redo{
  width: 65px; 
    height: 40px; 
    background-color: #282828; 
    color: #fff; 
    border: none; 
    border-radius: 5px; 
    cursor: pointer; 
}
.redo svg{
  fill: #fff; 
    width: 48px; 
    height: 28px; 
    margin-right: 5px; 
}
  .undo {
    width: 65px; 
    height: 40px; 
    background-color: #282828; 
    color: #fff; 
    border: none; 
    border-radius: 5px; 
    cursor: pointer; 
  }

  .undo svg {
    fill: #fff; 
    width: 48px; 
    height: 28px; 
    margin-right: 5px; 
  }

.formatHeader{
  width: 65px; 
    height: 40px; 
    background-color: #282828; 
    color: #fff; 
    border: none; 
    border-radius: 5px; 
    cursor: pointer; 
}
.formatHeader svg{
  fill: #fff; 
    width: 48px; 
    height: 28px; 
    
}
.formatParagraph{
  width: 65px; 
    height: 40px; 
    background-color: #282828; 
    color: #fff; 
    border: none; 
    border-radius: 5px; 
    cursor: pointer; 
}
.formatParagraph svg{
  fill: #fff; 
    width: 48px; 
    height: 28px; 
    margin-right: 5px; 
}
.insertImage{
  width: 65px; 
    height: 40px; 
    background-color: #282828; 
    color: #fff; 
    border: none; 
    border-radius: 5px; 
    cursor: pointer; 
}
.insertImage svg{
  fill: #fff; 
    width: 48px; 
    height: 28px; 
    margin-right: 5px; 
}
.copyHTML{
  color: #639EFF;
  background-color: #282828; 
  font-family: Roboto;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 23px; 
}
.toolbar {
  display: flex;
  margin-bottom: 10px;
  gap: 8px;
}


.content {
  border: 1px solid #ccc;
  padding: 10px;
  min-height: 200px;
}
</style>
