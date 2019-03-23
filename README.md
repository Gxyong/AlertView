# AlertView
弹窗，防iOS弹窗自定义控件
 #使用方法2，用于自定义的布局文件
     new BaseDialogFragment.Builder(this)
                .setContentView(R.layout.xxxxx)//布局文件
                .setAnimStyle(BaseDialog.AnimStyle.SCALE)
                //.setText(id, "我是预设置的文本")
                .setOnClickListener(R.id.vvvvv, new BaseDialog.OnClickListener<ImageView>() {
                    @Override
                    public void onClick(Dialog dialog, ImageView view) {
                        dialog.dismiss();
                    }
                })//控件的ID以及控件的点击事件
                .setOnClickListener(R.id.xxxxxx, new BaseDialog.OnClickListener() {
                    @Override
                    public void onClick(Dialog dialog, View view) {
                        ///**/
                    }
                })
                .show();
