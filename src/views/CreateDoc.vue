<template>
    <div>
<!--        <el-header>Header</el-header>-->
        <el-button type="primary" round>保存</el-button>
        <el-button type="info" round>返回</el-button>
        <br><br>
        <quill-editor
                v-model="content"
                ref="myQuillEditor"
                :options="editorOption"
                @blur="onEditorBlur($event)" @focus="onEditorFocus($event)"
                @change="onEditorChange($event)">
        </quill-editor>
    </div>

</template>
<script>
    // import { quillEditor } from 'vue-quill-editor'
    export default{
        data(){
            return {
                content:null,
                editorOption:{}
            }
        },
        methods:{
            onEditorBlur(){//失去焦点事件
            },
            onEditorFocus(){//获得焦点事件
            },
            onEditorChange(){//内容改变事件
            }
        }
    }
</script>