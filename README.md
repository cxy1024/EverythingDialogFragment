# EverythingDialogFragment

基类DialogFragment

使用方法(一)

```
  EverythingDialogFragment.
                newInstance().
                setWidthPercentSize(0.8f).
                setHeightPercentSize(0.8f).
                setContentView(R.layout.dialog_test).
                show(this).
                setConvertViewListener((holder, dialog) -> {
                    TextView tv1 = holder.findViewById(R.id.tv1);
                });
```
使用方法(二)
```
  EverythingDialogFragment.
                newInstance().
                setWidthPercentSize(0.8f).
                setHeightPercentSize(0.8f).
                setContentView(R.layout.dialog_test).
                addIdRes(R.id.tv1,R.id.tv2).
                show(this).
                setOnChildClickListener((dialog, v) -> {
                    if (R.id.tv1 == v.getId()){
                        //do something
                    }
                });
```


