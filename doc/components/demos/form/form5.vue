<template>
  <div>
    <Form :label-width="110" :model="data" ref="form" :rules="rules">
      <FormItem>
        <Checkbox v-model="required">是否必填</Checkbox>
      </FormItem>
      <!-- 
          这里定义的required属性会应用与验证规则中，适用于一些变动性的必填项。
         -->
      <FormItem label="自定义数组" prop="list[0]" :required="required">
        <input type="text" v-model="data.list[0]" />
      </FormItem>
      <FormItem label="自定义规则" prop="value" :required="required">
        <input type="text" v-model="data.value" />
      </FormItem>
      <FormItem :no-padding="true">
        <Button color="primary" @click="submit">提交</Button>
        <Button @click="reset">清除验证</Button>
      </FormItem>
    </Form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      required: true,
      data: {
        list: [null],
        value: null
      },
      rules: {}
    }
  },
  watch: {
    required() {
      this.$refs.form.reset();
    }
  },
  methods: {
    submit() {
      let validResult = this.$refs.form.valid();
      if (validResult.result) {
        this.$Message("验证成功");
      } else {
        this.$Message.error(`还有${validResult.messages.length}个错误未通过验证。`);
      }
    },
    reset() {
      this.$refs.form.reset();
    },
  }
};
</script>