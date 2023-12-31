# classes.dex

.class public final synthetic Lapp/a/module_ai/O0OO;
.super Ljava/lang/Object;
.source "R8$$SyntheticClass"

# interfaces
.implements Landroidx/lifecycle/Observer;


# instance fields
.field public final synthetic OOOO:I

.field public final synthetic OOOo:Ljava/lang/Object;


# direct methods
.method public synthetic constructor <init>(Ljava/lang/Object;I)V
    .registers 3

    .line 1
    iput p2, p0, Lapp/a/module_ai/O0OO;->OOOO:I

    iput-object p1, p0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    invoke-direct {p0}, Ljava/lang/Object;-><init>()V

    return-void
.end method


# virtual methods
.method public final onChanged(Ljava/lang/Object;)V
    .registers 38

    move-object/from16 v0, p0

    iget v1, v0, Lapp/a/module_ai/O0OO;->OOOO:I

    const/4 v2, 0x0

    const/4 v3, 0x1

    const/4 v4, 0x0

    const/16 v5, 0x64

    const/4 v6, 0x6

    const-string v7, ""

    const-string v8, "adapter"

    const/4 v9, 0x2

    const-string v10, "it"

    const/16 v11, 0xa

    const-string v12, "this$0"

    packed-switch v1, :pswitch_data_c08

    goto/16 :goto_bec

    :pswitch_1a  #0x1c
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/question/QuestionActivity;

    move-object/from16 v2, p1

    check-cast v2, Ljava/util/List;

    sget v3, Lcom/caoliu/module_mine/question/QuestionActivity;->O0oo:I

    .line 1
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 2
    iget-object v3, v1, Lcom/caoliu/module_mine/question/QuestionActivity;->O0OO:Ljava/util/ArrayList;

    invoke-virtual {v3}, Ljava/util/ArrayList;->clear()V

    .line 3
    iget-object v3, v1, Lcom/caoliu/module_mine/question/QuestionActivity;->O0OO:Ljava/util/ArrayList;

    invoke-static {v2, v10}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    .line 4
    new-instance v4, Ljava/util/ArrayList;

    invoke-static {v2, v11}, Lkotlin/collections/OO00O;->OO0oO(Ljava/lang/Iterable;I)I

    move-result v5

    invoke-direct {v4, v5}, Ljava/util/ArrayList;-><init>(I)V

    .line 5
    invoke-interface {v2}, Ljava/lang/Iterable;->iterator()Ljava/util/Iterator;

    move-result-object v2

    :goto_3e
    invoke-interface {v2}, Ljava/util/Iterator;->hasNext()Z

    move-result v5

    if-eqz v5, :cond_52

    invoke-interface {v2}, Ljava/util/Iterator;->next()Ljava/lang/Object;

    move-result-object v5

    .line 6
    check-cast v5, Lcom/caoliu/lib_common/entity/FileResponse;

    .line 7
    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/FileResponse;->getUrl()Ljava/lang/String;

    move-result-object v5

    invoke-virtual {v4, v5}, Ljava/util/ArrayList;->add(Ljava/lang/Object;)Z

    goto :goto_3e

    :cond_52
    invoke-virtual {v3, v4}, Ljava/util/ArrayList;->addAll(Ljava/util/Collection;)Z

    .line 8
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->O0OO()Lcom/caoliu/lib_common/base/BaseViewModel;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_mine/mine/MineViewModel;

    .line 9
    iget v3, v1, Lcom/caoliu/module_mine/question/QuestionActivity;->O0oO:I

    .line 10
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityQuestionBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityQuestionBinding;->OoOo:Landroid/widget/EditText;

    invoke-virtual {v4}, Landroid/widget/EditText;->getText()Landroid/text/Editable;

    move-result-object v4

    invoke-virtual {v4}, Ljava/lang/Object;->toString()Ljava/lang/String;

    move-result-object v4

    .line 11
    iget-object v1, v1, Lcom/caoliu/module_mine/question/QuestionActivity;->O0OO:Ljava/util/ArrayList;

    .line 12
    invoke-virtual {v2, v3, v4, v1}, Lcom/caoliu/module_mine/mine/MineViewModel;->oOO0(ILjava/lang/String;Ljava/util/ArrayList;)V

    return-void

    .line 13
    :pswitch_73  #0x1b
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/pwd/BindPhoneFragment;

    move-object/from16 v2, p1

    check-cast v2, Ljava/lang/Boolean;

    sget v2, Lcom/caoliu/module_mine/pwd/BindPhoneFragment;->O0O0:I

    .line 14
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 15
    iget-object v1, v1, Lcom/caoliu/module_mine/pwd/BindPhoneFragment;->O0Oo:Lcom/caoliu/module_mine/pwd/BindPhoneFragment$OOOO;

    invoke-virtual {v1, v3}, Landroid/os/Handler;->sendEmptyMessage(I)Z

    return-void

    .line 16
    :pswitch_86  #0x1a
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/pwd/BindPhoneActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_mine/pwd/BindPhoneActivity;->O0OO:I

    .line 17
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 18
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v3

    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    .line 19
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getShowMsg()Ljava/lang/String;

    move-result-object v3

    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oo(Ljava/lang/String;)V

    .line 20
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getSuccess()Z

    move-result v2

    if-eqz v2, :cond_c7

    .line 21
    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->O0Oo()Lcom/caoliu/lib_common/entity/IUserInfo;

    move-result-object v2

    if-nez v2, :cond_ae

    goto :goto_c1

    .line 22
    :cond_ae
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v3

    check-cast v3, Lcom/caoliu/module_mine/databinding/ActivityBindPhoneBinding;

    iget-object v3, v3, Lcom/caoliu/module_mine/databinding/ActivityBindPhoneBinding;->OoOo:Landroid/widget/EditText;

    invoke-virtual {v3}, Landroid/widget/EditText;->getText()Landroid/text/Editable;

    move-result-object v3

    invoke-virtual {v3}, Ljava/lang/Object;->toString()Ljava/lang/String;

    move-result-object v3

    invoke-virtual {v2, v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->setPhoneNumber(Ljava/lang/String;)V

    .line 23
    :goto_c1
    invoke-static {v2}, Lcom/caoliu/lib_common/ExKt;->ooO0(Lcom/caoliu/lib_common/entity/IUserInfo;)V

    .line 24
    invoke-virtual {v1}, Landroid/app/Activity;->finish()V

    :cond_c7
    return-void

    .line 25
    :pswitch_c8  #0x19
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/proxy/ProxyActivity;

    move-object/from16 v2, p1

    check-cast v2, Ljava/util/List;

    sget v3, Lcom/caoliu/module_mine/proxy/ProxyActivity;->Oo0o:I

    .line 26
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 27
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v3

    check-cast v3, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;

    iget-object v3, v3, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;->Oo00:Landroid/widget/TextView;

    new-instance v6, Ljava/lang/StringBuilder;

    invoke-direct {v6}, Ljava/lang/StringBuilder;-><init>()V

    const-string v7, "你直接推广的所有用户会员或金币充值，都将获得直接收益。代理收益根据金额分为"

    invoke-virtual {v6, v7}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v7

    invoke-virtual {v6, v7}, Ljava/lang/StringBuilder;->append(I)Ljava/lang/StringBuilder;

    const-string v7, "个档位，具体如下："

    invoke-virtual {v6, v7}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v6}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v6

    invoke-virtual {v3, v6}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 28
    new-instance v3, Ljava/lang/StringBuffer;

    invoke-direct {v3}, Ljava/lang/StringBuffer;-><init>()V

    .line 29
    new-instance v6, Ljava/lang/StringBuffer;

    invoke-direct {v6}, Ljava/lang/StringBuffer;-><init>()V

    .line 30
    invoke-static {v2}, LO0oOo/O00OO0;->oO00(Ljava/util/Collection;)LOOO0oo/OOO0OO;

    move-result-object v7

    .line 31
    invoke-virtual {v7}, LOOO0oo/OOOO0O;->OOOO()Lkotlin/collections/O0000;

    move-result-object v7

    .line 32
    :cond_10c
    :goto_10c
    move-object v8, v7

    check-cast v8, LOOO0oo/OOOO00;

    .line 33
    iget-boolean v8, v8, LOOO0oo/OOOO00;->OooO:Z

    if-eqz v8, :cond_1d6

    .line 34
    invoke-virtual {v7}, Lkotlin/collections/O0000;->nextInt()I

    move-result v8

    .line 35
    invoke-interface {v2, v8}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v9

    check-cast v9, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v9}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getEarningEnd()Ljava/lang/String;

    move-result-object v9

    const-string v10, "0"

    invoke-static {v9, v10}, Lkotlin/jvm/internal/OO0O0;->OOOO(Ljava/lang/Object;Ljava/lang/Object;)Z

    move-result v9

    if-eqz v9, :cond_154

    .line 36
    new-instance v9, Ljava/lang/StringBuilder;

    invoke-direct {v9}, Ljava/lang/StringBuilder;-><init>()V

    const-string v10, "大于"

    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-interface {v2, v8}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v10

    check-cast v10, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v10}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getEarningStart()Ljava/lang/String;

    move-result-object v10

    if-eqz v10, :cond_148

    invoke-static {v10}, Ljava/lang/Double;->parseDouble(Ljava/lang/String;)D

    move-result-wide v10

    invoke-static {v10, v11}, Lcom/caoliu/lib_common/ExKt;->o0o0(D)Ljava/lang/String;

    move-result-object v10

    goto :goto_149

    :cond_148
    move-object v10, v4

    :goto_149
    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v9}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v6, v9}, Ljava/lang/StringBuffer;->append(Ljava/lang/String;)Ljava/lang/StringBuffer;

    goto :goto_197

    .line 37
    :cond_154
    new-instance v9, Ljava/lang/StringBuilder;

    invoke-direct {v9}, Ljava/lang/StringBuilder;-><init>()V

    invoke-interface {v2, v8}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v10

    check-cast v10, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v10}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getEarningStart()Ljava/lang/String;

    move-result-object v10

    if-eqz v10, :cond_16e

    invoke-static {v10}, Ljava/lang/Double;->parseDouble(Ljava/lang/String;)D

    move-result-wide v10

    .line 38
    invoke-static {v10, v11}, Lcom/caoliu/lib_common/ExKt;->o0o0(D)Ljava/lang/String;

    move-result-object v10

    goto :goto_16f

    :cond_16e
    move-object v10, v4

    .line 39
    :goto_16f
    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    const-string v10, " - "

    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    .line 40
    invoke-interface {v2, v8}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v10

    check-cast v10, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v10}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getEarningEnd()Ljava/lang/String;

    move-result-object v10

    if-eqz v10, :cond_18c

    invoke-static {v10}, Ljava/lang/Double;->parseDouble(Ljava/lang/String;)D

    move-result-wide v10

    invoke-static {v10, v11}, Lcom/caoliu/lib_common/ExKt;->o0o0(D)Ljava/lang/String;

    move-result-object v10

    goto :goto_18d

    :cond_18c
    move-object v10, v4

    .line 41
    :goto_18d
    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v9}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v9

    .line 42
    invoke-virtual {v6, v9}, Ljava/lang/StringBuffer;->append(Ljava/lang/String;)Ljava/lang/StringBuffer;

    .line 43
    :goto_197
    new-instance v9, Ljava/lang/StringBuilder;

    invoke-direct {v9}, Ljava/lang/StringBuilder;-><init>()V

    invoke-interface {v2, v8}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v10

    check-cast v10, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v10}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getProportion()Ljava/lang/String;

    move-result-object v10

    if-eqz v10, :cond_1b4

    invoke-static {v10}, Ljava/lang/Double;->parseDouble(Ljava/lang/String;)D

    move-result-wide v10

    int-to-double v12, v5

    mul-double v10, v10, v12

    invoke-static {v10, v11}, Lcom/caoliu/lib_common/ExKt;->o0o0(D)Ljava/lang/String;

    move-result-object v10

    goto :goto_1b5

    :cond_1b4
    move-object v10, v4

    :goto_1b5
    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    const/16 v10, 0x25

    invoke-virtual {v9, v10}, Ljava/lang/StringBuilder;->append(C)Ljava/lang/StringBuilder;

    invoke-virtual {v9}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v3, v9}, Ljava/lang/StringBuffer;->append(Ljava/lang/String;)Ljava/lang/StringBuffer;

    .line 44
    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v9

    add-int/lit8 v9, v9, -0x1

    if-eq v8, v9, :cond_10c

    const-string v8, "\n"

    .line 45
    invoke-virtual {v6, v8}, Ljava/lang/StringBuffer;->append(Ljava/lang/String;)Ljava/lang/StringBuffer;

    .line 46
    invoke-virtual {v3, v8}, Ljava/lang/StringBuffer;->append(Ljava/lang/String;)Ljava/lang/StringBuffer;

    goto/16 :goto_10c

    .line 47
    :cond_1d6
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;

    iget-object v2, v2, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;->Ooo0:Landroid/widget/TextView;

    invoke-virtual {v6}, Ljava/lang/StringBuffer;->toString()Ljava/lang/String;

    move-result-object v4

    invoke-virtual {v2, v4}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 48
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;

    iget-object v1, v1, Lcom/caoliu/module_mine/databinding/ActivityProxyBinding;->Oo0O:Landroid/widget/TextView;

    invoke-virtual {v3}, Ljava/lang/StringBuffer;->toString()Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    return-void

    .line 49
    :pswitch_1f5  #0x18
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/mine/V2MineFragment;

    move-object/from16 v2, p1

    check-cast v2, Ljava/util/List;

    sget v3, Lcom/caoliu/module_mine/mine/V2MineFragment;->O0OO:I

    .line 50
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 51
    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v3

    if-lez v3, :cond_246

    .line 52
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_mine/databinding/FragmentV2MineBinding;

    iget-object v1, v1, Lcom/caoliu/module_mine/databinding/FragmentV2MineBinding;->oO00:Landroid/widget/TextView;

    new-instance v3, Ljava/lang/StringBuilder;

    invoke-direct {v3}, Ljava/lang/StringBuilder;-><init>()V

    const-string v6, "返利最高"

    invoke-virtual {v3, v6}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    .line 53
    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v6

    add-int/lit8 v6, v6, -0x1

    invoke-interface {v2, v6}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v2

    check-cast v2, Lcom/caoliu/lib_common/entity/EarningSettingResponse;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/EarningSettingResponse;->getProportion()Ljava/lang/String;

    move-result-object v2

    if-eqz v2, :cond_237

    invoke-static {v2}, Ljava/lang/Double;->parseDouble(Ljava/lang/String;)D

    move-result-wide v6

    int-to-double v4, v5

    mul-double v6, v6, v4

    invoke-static {v6, v7}, Lcom/caoliu/lib_common/ExKt;->o0o0(D)Ljava/lang/String;

    move-result-object v4

    .line 54
    :cond_237
    invoke-virtual {v3, v4}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    const-string v2, "%！\n零成本实现百万梦想"

    invoke-virtual {v3, v2}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v3}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    :cond_246
    return-void

    .line 55
    :pswitch_247  #0x17
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/mine/MineFragment;

    move-object/from16 v3, p1

    check-cast v3, Lcom/caoliu/lib_common/entity/IUserInfo;

    sget v5, Lcom/caoliu/module_mine/mine/MineFragment;->O0OO:I

    .line 56
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 57
    invoke-static {}, Lcom/blankj/utilcode/util/SPUtils;->getInstance()Lcom/blankj/utilcode/util/SPUtils;

    move-result-object v5

    const v8, 0x186a0

    const-string v9, "coinvideofree"

    invoke-virtual {v5, v9, v8}, Lcom/blankj/utilcode/util/SPUtils;->getInt(Ljava/lang/String;I)I

    move-result v5

    .line 58
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->O00O:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v8}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OOOO()Lo0o0O/O0O00;

    .line 59
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->OooO:Lcom/caoliu/lib_common/widget/HeadView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getHeadUrl()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getVipFlag()Z

    move-result v10

    invoke-virtual {v8, v9, v10}, Lcom/caoliu/lib_common/widget/HeadView;->OOOo(Ljava/lang/String;Z)V

    .line 60
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->oOoO:Landroid/widget/TextView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getNickName()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v8, v9}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 61
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->oOOo:Landroid/widget/TextView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowers()J

    move-result-wide v9

    invoke-static {v9, v10}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v8, v9}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 62
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->oOO0:Landroid/widget/TextView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowed()J

    move-result-wide v9

    invoke-static {v9, v10}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v8, v9}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 63
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->oO00:Lcom/caoliu/lib_common/widget/VipView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getExpLevel()I

    move-result v9

    invoke-virtual {v8, v9}, Lcom/caoliu/lib_common/widget/VipView;->setVipLevel(I)V

    .line 64
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v8

    check-cast v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v8, v8, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->O000:Landroid/widget/TextView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getCoinBalance()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v8, v9}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 65
    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->O0Oo()Lcom/caoliu/lib_common/entity/IUserInfo;

    move-result-object v8

    if-eqz v8, :cond_2dd

    invoke-virtual {v8}, Lcom/caoliu/lib_common/entity/IUserInfo;->getVipEnd()Ljava/lang/String;

    move-result-object v8

    goto :goto_2de

    :cond_2dd
    move-object v8, v4

    :goto_2de
    invoke-static {v8}, Ljava/lang/String;->valueOf(Ljava/lang/Object;)Ljava/lang/String;

    move-result-object v8

    const-string v9, " "

    .line 66
    filled-new-array {v9}, [Ljava/lang/String;

    move-result-object v9

    invoke-static {v8, v9, v2, v2, v6}, Lkotlin/text/OOO00;->OooOo(Ljava/lang/CharSequence;[Ljava/lang/String;ZII)Ljava/util/List;

    move-result-object v6

    .line 67
    invoke-interface {v6}, Ljava/util/List;->size()I

    move-result v8

    const-string v9, "会员有效期："

    if-lez v8, :cond_30a

    .line 68
    new-instance v4, Ljava/lang/StringBuilder;

    invoke-direct {v4}, Ljava/lang/StringBuilder;-><init>()V

    invoke-virtual {v4, v9}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-interface {v6, v2}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v2

    check-cast v2, Ljava/lang/String;

    invoke-virtual {v4, v2}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v4}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v2

    goto :goto_323

    .line 69
    :cond_30a
    new-instance v2, Ljava/lang/StringBuilder;

    invoke-direct {v2}, Ljava/lang/StringBuilder;-><init>()V

    invoke-virtual {v2, v9}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->O0Oo()Lcom/caoliu/lib_common/entity/IUserInfo;

    move-result-object v6

    if-eqz v6, :cond_31c

    invoke-virtual {v6}, Lcom/caoliu/lib_common/entity/IUserInfo;->getVipEnd()Ljava/lang/String;

    move-result-object v4

    :cond_31c
    invoke-virtual {v2, v4}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v2}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v2

    .line 70
    :goto_323
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;

    iget-object v1, v1, Lcom/caoliu/module_mine/databinding/FragmentMineBinding;->oOoo:Landroid/widget/TextView;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getVipFlag()Z

    move-result v4

    if-eqz v4, :cond_349

    .line 71
    new-instance v4, Ljava/lang/StringBuilder;

    invoke-direct {v4}, Ljava/lang/StringBuilder;-><init>()V

    invoke-virtual {v4, v2}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->getExpLevel()I

    move-result v2

    if-lt v2, v5, :cond_341

    const-string v7, "，金币视频免费"

    :cond_341
    invoke-virtual {v4, v7}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v4}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v2

    goto :goto_34b

    :cond_349
    const-string v2, "您当前还不是VIP，立即开通吧"

    .line 72
    :goto_34b
    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    return-void

    .line 73
    :pswitch_34f  #0x16
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/mine/EditInfoActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_mine/mine/EditInfoActivity;->Oo00:I

    .line 74
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 75
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    return-void

    .line 76
    :pswitch_364  #0x15
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/mine/ChangeNameOrSignActivity;

    move-object/from16 v2, p1

    check-cast v2, Ljava/lang/Boolean;

    sget v2, Lcom/caoliu/module_mine/mine/ChangeNameOrSignActivity;->Oo00:I

    .line 77
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 78
    invoke-static {}, LOOoO0O/O0O0O;->OOOo()LOOoO0O/O0O0O;

    move-result-object v2

    .line 79
    new-instance v3, Lcom/caoliu/lib_utils/event/MessageEvent;

    sget-object v4, Ljava/lang/Boolean;->TRUE:Ljava/lang/Boolean;

    const/16 v5, 0x2719

    invoke-direct {v3, v5, v4}, Lcom/caoliu/lib_utils/event/MessageEvent;-><init>(ILjava/lang/Object;)V

    invoke-virtual {v2, v3}, LOOoO0O/O0O0O;->OOo0(Ljava/lang/Object;)V

    const-string v2, "修改成功"

    .line 80
    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oo(Ljava/lang/String;)V

    .line 81
    invoke-virtual {v1}, Landroid/app/Activity;->finish()V

    return-void

    .line 82
    :pswitch_38a  #0x14
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/level/MyLevelActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/entity/UserExpResponse;

    sget v4, Lcom/caoliu/module_mine/level/MyLevelActivity;->Oo0O:I

    .line 83
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 84
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->OoOo:Landroid/widget/ProgressBar;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getEnd()I

    move-result v5

    add-int/2addr v5, v3

    invoke-virtual {v4, v5}, Landroid/widget/ProgressBar;->setMax(I)V

    .line 85
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->OoOo:Landroid/widget/ProgressBar;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getCurrentExp()I

    move-result v5

    if-ge v5, v3, :cond_3b7

    const/4 v5, 0x1

    goto :goto_3bb

    :cond_3b7
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getCurrentExp()I

    move-result v5

    :goto_3bb
    invoke-virtual {v4, v5}, Landroid/widget/ProgressBar;->setProgress(I)V

    .line 86
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->OooO:Landroid/widget/TextView;

    new-instance v5, Ljava/lang/StringBuilder;

    invoke-direct {v5}, Ljava/lang/StringBuilder;-><init>()V

    const/16 v6, 0x76

    invoke-virtual {v5, v6}, Ljava/lang/StringBuilder;->append(C)Ljava/lang/StringBuilder;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getLevel()I

    move-result v7

    invoke-virtual {v5, v7}, Ljava/lang/StringBuilder;->append(I)Ljava/lang/StringBuilder;

    invoke-virtual {v5}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v5

    invoke-virtual {v4, v5}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 87
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->Ooo0:Landroid/widget/TextView;

    new-instance v5, Ljava/lang/StringBuilder;

    invoke-direct {v5}, Ljava/lang/StringBuilder;-><init>()V

    invoke-virtual {v5, v6}, Ljava/lang/StringBuilder;->append(C)Ljava/lang/StringBuilder;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getLevel()I

    move-result v6

    add-int/2addr v6, v3

    invoke-virtual {v5, v6}, Ljava/lang/StringBuilder;->append(I)Ljava/lang/StringBuilder;

    invoke-virtual {v5}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v5

    invoke-virtual {v4, v5}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 88
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v4, v4, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->Oooo:Landroid/widget/TextView;

    .line 89
    new-instance v5, Ljava/lang/StringBuilder;

    invoke-direct {v5}, Ljava/lang/StringBuilder;-><init>()V

    const-string v6, "距离"

    invoke-virtual {v5, v6}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getLevel()I

    move-result v6

    add-int/2addr v6, v3

    invoke-virtual {v5, v6}, Ljava/lang/StringBuilder;->append(I)Ljava/lang/StringBuilder;

    const-string v3, "级还差"

    invoke-virtual {v5, v3}, Ljava/lang/StringBuilder;->append(Ljava/lang/String;)Ljava/lang/StringBuilder;

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;

    iget-object v1, v1, Lcom/caoliu/module_mine/databinding/ActivityMyLevelBinding;->OoOo:Landroid/widget/ProgressBar;

    invoke-virtual {v1}, Landroid/widget/ProgressBar;->getMax()I

    move-result v1

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/UserExpResponse;->getCurrentExp()I

    move-result v2

    sub-int/2addr v1, v2

    invoke-virtual {v5, v1}, Ljava/lang/StringBuilder;->append(I)Ljava/lang/StringBuilder;

    const/16 v1, 0x70b9

    invoke-virtual {v5, v1}, Ljava/lang/StringBuilder;->append(C)Ljava/lang/StringBuilder;

    invoke-virtual {v5}, Ljava/lang/StringBuilder;->toString()Ljava/lang/String;

    move-result-object v1

    .line 90
    invoke-virtual {v4, v1}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    return-void

    .line 91
    :pswitch_43d  #0x13
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/fans/FansActivity;

    move-object/from16 v2, p1

    check-cast v2, Ljava/lang/Boolean;

    sget v2, Lcom/caoliu/module_mine/fans/FansActivity;->O0oO:I

    .line 92
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 93
    iget v2, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo00:I

    const/4 v3, 0x3

    if-ne v2, v3, :cond_474

    .line 94
    iget-object v2, v1, Lcom/caoliu/module_mine/fans/FansActivity;->O0O0:Lcom/caoliu/module_mine/fans/SeenAdapter;

    const-string v3, "seenAdapter"

    if-eqz v2, :cond_470

    iget v5, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0o:I

    invoke-virtual {v2, v5}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->getItem(I)Ljava/lang/Object;

    move-result-object v2

    check-cast v2, Lcom/caoliu/lib_common/entity/WhoHasSeenResponse$Data;

    iget-boolean v5, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0O:Z

    invoke-virtual {v2, v5}, Lcom/caoliu/lib_common/entity/WhoHasSeenResponse$Data;->setFollow(Z)V

    .line 95
    iget-object v2, v1, Lcom/caoliu/module_mine/fans/FansActivity;->O0O0:Lcom/caoliu/module_mine/fans/SeenAdapter;

    if-eqz v2, :cond_46c

    iget v1, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0o:I

    invoke-virtual {v2, v1}, Landroidx/recyclerview/widget/RecyclerView$Adapter;->notifyItemChanged(I)V

    goto :goto_48e

    :cond_46c
    invoke-static {v3}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 96
    :cond_470
    invoke-static {v3}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 97
    :cond_474
    iget-object v2, v1, Lcom/caoliu/module_mine/fans/FansActivity;->O0Oo:Lcom/caoliu/module_mine/fans/FansAdapter;

    if-eqz v2, :cond_493

    iget v3, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0o:I

    invoke-virtual {v2, v3}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->getItem(I)Ljava/lang/Object;

    move-result-object v2

    check-cast v2, Lcom/caoliu/lib_common/entity/IUserInfo;

    iget-boolean v3, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0O:Z

    invoke-virtual {v2, v3}, Lcom/caoliu/lib_common/entity/IUserInfo;->setFollowFlag(Z)V

    .line 98
    iget-object v2, v1, Lcom/caoliu/module_mine/fans/FansActivity;->O0Oo:Lcom/caoliu/module_mine/fans/FansAdapter;

    if-eqz v2, :cond_48f

    iget v1, v1, Lcom/caoliu/module_mine/fans/FansActivity;->Oo0o:I

    invoke-virtual {v2, v1}, Landroidx/recyclerview/widget/RecyclerView$Adapter;->notifyItemChanged(I)V

    :goto_48e
    return-void

    :cond_48f
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 99
    :cond_493
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 100
    :pswitch_497  #0x12
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/black/BlackUserActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_mine/black/BlackUserActivity;->Oo00:I

    .line 101
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 102
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v3

    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    .line 103
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getShowMsg()Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oo(Ljava/lang/String;)V

    return-void

    .line 104
    :pswitch_4b3  #0x11
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/user/V3UserCenterActivity;

    move-object/from16 v2, p1

    check-cast v2, Ljava/lang/Boolean;

    sget v2, Lcom/caoliu/module_main/user/V3UserCenterActivity;->O0Oo:I

    .line 105
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 106
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    invoke-virtual {v2}, Landroid/widget/TextView;->getText()Ljava/lang/CharSequence;

    move-result-object v2

    invoke-virtual {v2}, Ljava/lang/Object;->toString()Ljava/lang/String;

    move-result-object v2

    sget v3, Lcom/caoliu/lib_resource/R$string;->string_add_follow:I

    invoke-virtual {v1, v3}, Landroid/app/Activity;->getString(I)Ljava/lang/String;

    move-result-object v4

    invoke-static {v2, v4}, Lkotlin/jvm/internal/OO0O0;->OOOO(Ljava/lang/Object;Ljava/lang/Object;)Z

    move-result v2

    const-wide/16 v4, 0x1

    if-eqz v2, :cond_569

    .line 107
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    invoke-virtual {v1}, Landroidx/appcompat/app/AppCompatActivity;->getResources()Landroid/content/res/Resources;

    move-result-object v3

    sget v6, Lcom/caoliu/lib_resource/R$color;->white:I

    invoke-virtual {v3, v6}, Landroid/content/res/Resources;->getColor(I)I

    move-result v3

    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setTextColor(I)V

    .line 108
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    .line 109
    sget v3, Lcom/caoliu/lib_resource/R$string;->text_following:I

    invoke-virtual {v1, v3}, Landroid/app/Activity;->getString(I)Ljava/lang/String;

    move-result-object v3

    .line 110
    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 111
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    sget v3, Lcom/caoliu/lib_resource/R$drawable;->rec_25_accent:I

    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setBackgroundResource(I)V

    .line 112
    iget-object v2, v1, Lcom/caoliu/module_main/user/V3UserCenterActivity;->Oo0o:Lcom/caoliu/lib_common/entity/IUserInfo;

    if-eqz v2, :cond_5ed

    .line 113
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getUserId()Ljava/lang/String;

    move-result-object v3

    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->o0oo()Ljava/lang/String;

    move-result-object v6

    invoke-static {v3, v6}, Lkotlin/jvm/internal/OO0O0;->OOOO(Ljava/lang/Object;Ljava/lang/Object;)Z

    move-result v3

    if-eqz v3, :cond_54a

    .line 114
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowed()J

    move-result-wide v6

    add-long/2addr v6, v4

    invoke-virtual {v2, v6, v7}, Lcom/caoliu/lib_common/entity/IUserInfo;->setFollowed(J)V

    .line 115
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Oo0O:Landroid/widget/TextView;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowed()J

    move-result-wide v2

    invoke-static {v2, v3}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    goto/16 :goto_5ed

    .line 116
    :cond_54a
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowers()J

    move-result-wide v6

    add-long/2addr v6, v4

    invoke-virtual {v2, v6, v7}, Lcom/caoliu/lib_common/entity/IUserInfo;->setFollowers(J)V

    .line 117
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Oooo:Landroid/widget/TextView;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowers()J

    move-result-wide v2

    invoke-static {v2, v3}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    goto/16 :goto_5ed

    .line 118
    :cond_569
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    .line 119
    invoke-virtual {v1, v3}, Landroid/app/Activity;->getString(I)Ljava/lang/String;

    move-result-object v3

    .line 120
    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 121
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    invoke-virtual {v1}, Landroidx/appcompat/app/AppCompatActivity;->getResources()Landroid/content/res/Resources;

    move-result-object v3

    sget v6, Lcom/caoliu/lib_resource/R$color;->colorAccent:I

    invoke-virtual {v3, v6}, Landroid/content/res/Resources;->getColor(I)I

    move-result v3

    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setTextColor(I)V

    .line 122
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v2

    check-cast v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v2, v2, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Ooo0:Landroid/widget/TextView;

    sget v3, Lcom/caoliu/lib_resource/R$drawable;->rec_12_stroke_accent:I

    invoke-virtual {v2, v3}, Landroid/widget/TextView;->setBackgroundResource(I)V

    .line 123
    iget-object v2, v1, Lcom/caoliu/module_main/user/V3UserCenterActivity;->Oo0o:Lcom/caoliu/lib_common/entity/IUserInfo;

    if-eqz v2, :cond_5ed

    .line 124
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getUserId()Ljava/lang/String;

    move-result-object v3

    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->o0oo()Ljava/lang/String;

    move-result-object v6

    invoke-static {v3, v6}, Lkotlin/jvm/internal/OO0O0;->OOOO(Ljava/lang/Object;Ljava/lang/Object;)Z

    move-result v3

    if-eqz v3, :cond_5d0

    .line 125
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowed()J

    move-result-wide v6

    add-long/2addr v6, v4

    invoke-virtual {v2, v6, v7}, Lcom/caoliu/lib_common/entity/IUserInfo;->setFollowed(J)V

    .line 126
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Oo0O:Landroid/widget/TextView;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowed()J

    move-result-wide v2

    invoke-static {v2, v3}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    goto :goto_5ed

    .line 127
    :cond_5d0
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowers()J

    move-result-wide v6

    sub-long/2addr v6, v4

    invoke-virtual {v2, v6, v7}, Lcom/caoliu/lib_common/entity/IUserInfo;->setFollowers(J)V

    .line 128
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/ActivityV3UserCenterBinding;->OooO:Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/LayoutHeadDynamicUserV2Binding;->Oooo:Landroid/widget/TextView;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/IUserInfo;->getFollowers()J

    move-result-wide v2

    invoke-static {v2, v3}, Lcom/caoliu/lib_common/ExKt;->oOo0(J)Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    :cond_5ed
    :goto_5ed
    return-void

    .line 129
    :pswitch_5ee  #0x10
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/square/detail/BaoInfoActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_main/square/detail/BaoInfoActivity;->O0Oo:I

    .line 130
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 131
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    return-void

    .line 132
    :pswitch_603  #0xf
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/send/SendBaoFragment;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/entity/FileResponse;

    sget v4, Lcom/caoliu/module_main/send/SendBaoFragment;->oO00:I

    .line 133
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 134
    iget v4, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOOO:I

    add-int/2addr v4, v3

    iput v4, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOOO:I

    .line 135
    iget-object v4, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOoO:Ljava/util/ArrayList;

    invoke-virtual {v4}, Ljava/util/ArrayList;->clear()V

    .line 136
    iget v4, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOOO:I

    if-eq v4, v3, :cond_689

    if-eq v4, v9, :cond_622

    goto/16 :goto_6a4

    .line 137
    :cond_622
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/FileResponse;->getUrl()Ljava/lang/String;

    move-result-object v2

    iput-object v2, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOO0:Ljava/lang/String;

    .line 138
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->Oooo()Lcom/caoliu/lib_common/base/BaseViewModel;

    move-result-object v2

    move-object v12, v2

    check-cast v12, Lcom/caoliu/module_main/send/SendVideoViewModel;

    const/4 v14, 0x0

    .line 139
    iget-object v15, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOOo:Ljava/lang/String;

    .line 140
    iget-object v2, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->O0OO:Ljava/lang/String;

    .line 141
    iget-object v3, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOO0:Ljava/lang/String;

    .line 142
    iget-object v4, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOoO:Ljava/util/ArrayList;

    .line 143
    iget-object v5, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOoo:Ljava/util/ArrayList;

    .line 144
    new-instance v6, Ljava/util/ArrayList;

    invoke-static {v5, v11}, Lkotlin/collections/OO00O;->OO0oO(Ljava/lang/Iterable;I)I

    move-result v7

    invoke-direct {v6, v7}, Ljava/util/ArrayList;-><init>(I)V

    .line 145
    invoke-interface {v5}, Ljava/lang/Iterable;->iterator()Ljava/util/Iterator;

    move-result-object v5

    :goto_647
    invoke-interface {v5}, Ljava/util/Iterator;->hasNext()Z

    move-result v7

    if-eqz v7, :cond_65b

    invoke-interface {v5}, Ljava/util/Iterator;->next()Ljava/lang/Object;

    move-result-object v7

    .line 146
    check-cast v7, Lcom/caoliu/lib_common/entity/LabelResponse;

    .line 147
    invoke-virtual {v7}, Lcom/caoliu/lib_common/entity/LabelResponse;->getTagId()Ljava/lang/String;

    move-result-object v7

    invoke-virtual {v6, v7}, Ljava/util/ArrayList;->add(Ljava/lang/Object;)Z

    goto :goto_647

    :cond_65b
    const/16 v21, 0x1

    .line 148
    iget v5, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->O0oo:I

    move/from16 v22, v5

    const-wide/16 v23, 0x0

    .line 149
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/databinding/FragmentSendBaoBinding;

    iget-object v1, v1, Lcom/caoliu/module_main/databinding/FragmentSendBaoBinding;->OoO0:Landroid/widget/EditText;

    invoke-virtual {v1}, Landroid/widget/EditText;->getText()Landroid/text/Editable;

    move-result-object v1

    invoke-virtual {v1}, Ljava/lang/Object;->toString()Ljava/lang/String;

    move-result-object v25

    const/16 v26, 0x1

    const/16 v27, 0x0

    const/16 v28, 0x2000

    const-string v13, "0"

    const-string v16, ""

    move-object/from16 v17, v2

    move-object/from16 v18, v3

    move-object/from16 v19, v4

    move-object/from16 v20, v6

    .line 150
    invoke-static/range {v12 .. v28}, Lcom/caoliu/module_main/send/SendVideoViewModel;->OoOO(Lcom/caoliu/module_main/send/SendVideoViewModel;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/util/ArrayList;Ljava/util/ArrayList;IIJLjava/lang/String;III)V

    goto :goto_6a4

    .line 151
    :cond_689
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/FileResponse;->getUrl()Ljava/lang/String;

    move-result-object v2

    iput-object v2, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->oOOo:Ljava/lang/String;

    .line 152
    new-instance v2, Ljava/io/File;

    iget-object v3, v1, Lcom/caoliu/module_main/send/SendBaoFragment;->O0O0:Ljava/lang/String;

    invoke-direct {v2, v3}, Ljava/io/File;-><init>(Ljava/lang/String;)V

    .line 153
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->Oooo()Lcom/caoliu/lib_common/base/BaseViewModel;

    move-result-object v1

    check-cast v1, Lcom/caoliu/module_main/send/SendVideoViewModel;

    .line 154
    new-instance v3, Lcom/caoliu/module_main/send/OOOO;

    invoke-direct {v3}, Lcom/caoliu/module_main/send/OOOO;-><init>()V

    .line 155
    invoke-virtual {v1, v2, v3}, Lcom/caoliu/module_main/send/SendVideoViewModel;->OO0O(Ljava/io/File;LOOOoo/OOO0O;)V

    :goto_6a4
    return-void

    .line 156
    :pswitch_6a5  #0xe
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/report/ReportActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_main/report/ReportActivity;->O0o0:I

    .line 157
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 158
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    return-void

    .line 159
    :pswitch_6ba  #0xd
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/active/SendActiveShowActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_main/active/SendActiveShowActivity;->oOOo:I

    .line 160
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 161
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getShowMsg()Ljava/lang/String;

    move-result-object v3

    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oo(Ljava/lang/String;)V

    .line 162
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    return-void

    .line 163
    :pswitch_6d6  #0xc
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_main/active/ActiveDetailActivity;

    move-object/from16 v5, p1

    check-cast v5, Lcom/caoliu/lib_common/entity/ActiveResponse;

    sget v6, Lcom/caoliu/module_main/active/ActiveDetailActivity;->O0Oo:I

    .line 164
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 165
    iput-object v5, v1, Lcom/caoliu/module_main/active/ActiveDetailActivity;->O0OO:Lcom/caoliu/lib_common/entity/ActiveResponse;

    .line 166
    invoke-static {}, LOOoO0O/O0O0O;->OOOo()LOOoO0O/O0O0O;

    move-result-object v6

    new-instance v7, Lcom/caoliu/lib_utils/event/ActiveStatusEvent;

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getId()I

    move-result v9

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getJoined()Z

    move-result v10

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getActivityStatus()I

    move-result v12

    invoke-direct {v7, v9, v10, v12}, Lcom/caoliu/lib_utils/event/ActiveStatusEvent;-><init>(IZI)V

    invoke-virtual {v6, v7}, LOOoO0O/O0O0O;->OOo0(Ljava/lang/Object;)V

    .line 167
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v6

    check-cast v6, Lcom/caoliu/module_main/databinding/ActivityActiveDetailBinding;

    iget-object v6, v6, Lcom/caoliu/module_main/databinding/ActivityActiveDetailBinding;->OoOo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v6}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OOOO()Lo0o0O/O0O00;

    .line 168
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v6

    check-cast v6, Lcom/caoliu/module_main/databinding/ActivityActiveDetailBinding;

    iget-object v6, v6, Lcom/caoliu/module_main/databinding/ActivityActiveDetailBinding;->OoOo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v6}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OoOo()Lo0o0O/O0O00;

    .line 169
    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getList()Ljava/util/List;

    move-result-object v6

    invoke-interface {v6}, Ljava/lang/Iterable;->iterator()Ljava/util/Iterator;

    move-result-object v6

    :cond_71b
    invoke-interface {v6}, Ljava/util/Iterator;->hasNext()Z

    move-result v7

    if-eqz v7, :cond_74b

    invoke-interface {v6}, Ljava/util/Iterator;->next()Ljava/lang/Object;

    move-result-object v7

    move-object v9, v7

    check-cast v9, Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;

    invoke-virtual {v9}, Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;->getUserInfo()Lcom/caoliu/lib_common/entity/IUserInfo;

    move-result-object v9

    invoke-virtual {v9}, Lcom/caoliu/lib_common/entity/IUserInfo;->getUserId()Ljava/lang/String;

    move-result-object v9

    invoke-virtual {v9}, Ljava/lang/String;->toString()Ljava/lang/String;

    move-result-object v9

    invoke-static {}, Lcom/caoliu/lib_common/ExKt;->O0Oo()Lcom/caoliu/lib_common/entity/IUserInfo;

    move-result-object v10

    if-eqz v10, :cond_73f

    invoke-virtual {v10}, Lcom/caoliu/lib_common/entity/IUserInfo;->getUserId()Ljava/lang/String;

    move-result-object v10

    goto :goto_740

    :cond_73f
    move-object v10, v4

    :goto_740
    invoke-static {v10}, Ljava/lang/String;->valueOf(Ljava/lang/Object;)Ljava/lang/String;

    move-result-object v10

    invoke-static {v9, v10}, Lkotlin/jvm/internal/OO0O0;->OOOO(Ljava/lang/Object;Ljava/lang/Object;)Z

    move-result v9

    if-eqz v9, :cond_71b

    goto :goto_74c

    :cond_74b
    move-object v7, v4

    :goto_74c
    check-cast v7, Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;

    if-eqz v7, :cond_752

    const/4 v6, 0x1

    goto :goto_753

    :cond_752
    const/4 v6, 0x0

    .line 170
    :goto_753
    iput-boolean v6, v1, Lcom/caoliu/module_main/active/ActiveDetailActivity;->Oo0o:Z

    .line 171
    iget-object v6, v1, Lcom/caoliu/module_main/active/ActiveDetailActivity;->Oo0O:Lcom/caoliu/module_main/adapter/ActiveDetailAdapter;

    if-eqz v6, :cond_7a2

    new-array v3, v3, [Lcom/caoliu/lib_common/entity/ActiveInfoEntity;

    new-instance v7, Lcom/caoliu/lib_common/entity/ActiveInfoEntity;

    invoke-direct {v7, v4, v5}, Lcom/caoliu/lib_common/entity/ActiveInfoEntity;-><init>(Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;Lcom/caoliu/lib_common/entity/ActiveResponse;)V

    aput-object v7, v3, v2

    invoke-static {v3}, LO0oOo/O00OO0;->OO00([Ljava/lang/Object;)Ljava/util/ArrayList;

    move-result-object v2

    invoke-virtual {v6, v2}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->oOoO(Ljava/util/List;)V

    .line 172
    iget-object v2, v1, Lcom/caoliu/module_main/active/ActiveDetailActivity;->Oo0O:Lcom/caoliu/module_main/adapter/ActiveDetailAdapter;

    if-eqz v2, :cond_79e

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getList()Ljava/util/List;

    move-result-object v3

    .line 173
    new-instance v6, Ljava/util/ArrayList;

    invoke-static {v3, v11}, Lkotlin/collections/OO00O;->OO0oO(Ljava/lang/Iterable;I)I

    move-result v7

    invoke-direct {v6, v7}, Ljava/util/ArrayList;-><init>(I)V

    .line 174
    invoke-interface {v3}, Ljava/lang/Iterable;->iterator()Ljava/util/Iterator;

    move-result-object v3

    :goto_77e
    invoke-interface {v3}, Ljava/util/Iterator;->hasNext()Z

    move-result v7

    if-eqz v7, :cond_793

    invoke-interface {v3}, Ljava/util/Iterator;->next()Ljava/lang/Object;

    move-result-object v7

    .line 175
    check-cast v7, Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;

    .line 176
    new-instance v8, Lcom/caoliu/lib_common/entity/ActiveInfoEntity;

    invoke-direct {v8, v7, v4}, Lcom/caoliu/lib_common/entity/ActiveInfoEntity;-><init>(Lcom/caoliu/lib_common/entity/ActiveResponse$ActiveOrderShow;Lcom/caoliu/lib_common/entity/ActiveResponse;)V

    invoke-virtual {v6, v8}, Ljava/util/ArrayList;->add(Ljava/lang/Object;)Z

    goto :goto_77e

    :cond_793
    invoke-virtual {v2, v6}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->OO0O(Ljava/util/Collection;)V

    .line 177
    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ActiveResponse;->getJoined()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/module_main/active/ActiveDetailActivity;->O00o(Z)V

    return-void

    .line 178
    :cond_79e
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 179
    :cond_7a2
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 180
    :pswitch_7a6  #0xb
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_im/message/LikeFragment;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/entity/CommentMessageResponse;

    sget v5, Lcom/caoliu/module_im/message/LikeFragment;->O0oO:I

    .line 181
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 182
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lcom/caoliu/module_im/databinding/FragmentLikeBinding;

    iget-object v5, v5, Lcom/caoliu/module_im/databinding/FragmentLikeBinding;->OoOo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v5}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OOOO()Lo0o0O/O0O00;

    .line 183
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lcom/caoliu/module_im/databinding/FragmentLikeBinding;

    iget-object v5, v5, Lcom/caoliu/module_im/databinding/FragmentLikeBinding;->OoOo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v5}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OoOo()Lo0o0O/O0O00;

    .line 184
    iget v5, v1, Lcom/caoliu/module_im/message/LikeFragment;->O0OO:I

    if-ne v5, v3, :cond_7e6

    .line 185
    iget-object v3, v1, Lcom/caoliu/module_im/message/LikeFragment;->O0O0:Lcom/caoliu/module_im/message/MessageLikeAdapter;

    if-eqz v3, :cond_7e2

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/CommentMessageResponse;->getDataList()Ljava/util/List;

    move-result-object v2

    const-string v5, "null cannot be cast to non-null type kotlin.collections.MutableList<com.caoliu.lib_common.entity.CommentMessage>"

    invoke-static {v2, v5}, Lkotlin/jvm/internal/OO0O0;->OOoO(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-static {v2}, Lkotlin/jvm/internal/O0O0O;->OOOO(Ljava/lang/Object;)Ljava/util/List;

    move-result-object v2

    invoke-virtual {v3, v2}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->oOoO(Ljava/util/List;)V

    goto :goto_7f1

    :cond_7e2
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 186
    :cond_7e6
    iget-object v3, v1, Lcom/caoliu/module_im/message/LikeFragment;->O0O0:Lcom/caoliu/module_im/message/MessageLikeAdapter;

    if-eqz v3, :cond_801

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/CommentMessageResponse;->getDataList()Ljava/util/List;

    move-result-object v2

    invoke-virtual {v3, v2}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->OO0O(Ljava/util/Collection;)V

    .line 187
    :goto_7f1
    iget-object v2, v1, Lcom/caoliu/module_im/message/LikeFragment;->O0O0:Lcom/caoliu/module_im/message/MessageLikeAdapter;

    if-eqz v2, :cond_7fd

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OOoo()Landroid/view/View;

    move-result-object v1

    invoke-virtual {v2, v1}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->oOO0(Landroid/view/View;)V

    return-void

    :cond_7fd
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 188
    :cond_801
    invoke-static {v8}, Lkotlin/jvm/internal/OO0O0;->Ooo0(Ljava/lang/String;)V

    throw v4

    .line 189
    :pswitch_805  #0xa
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_im/chat/ChatNewActivity;

    move-object/from16 v5, p1

    check-cast v5, Lcom/caoliu/module_im/entity/ImResponse;

    sget v6, Lcom/caoliu/module_im/chat/ChatNewActivity;->O00o:I

    .line 190
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 191
    invoke-virtual {v5}, Lcom/caoliu/module_im/entity/ImResponse;->getList()Ljava/util/List;

    move-result-object v5

    .line 192
    invoke-virtual {v1}, Lcom/caoliu/module_im/chat/ChatNewActivity;->O000()Lcom/caoliu/module_im/adapter/ChatNewAdapter;

    move-result-object v6

    invoke-virtual {v6, v5}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->OO0O(Ljava/util/Collection;)V

    .line 193
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lcom/caoliu/module_im/databinding/ActivityChatNewBinding;

    iget-object v5, v5, Lcom/caoliu/module_im/databinding/ActivityChatNewBinding;->OooO:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v5}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OOOO()Lo0o0O/O0O00;

    .line 194
    invoke-virtual {v1}, Lcom/caoliu/module_im/chat/ChatNewActivity;->O000()Lcom/caoliu/module_im/adapter/ChatNewAdapter;

    move-result-object v5

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo0O()Landroid/view/View;

    move-result-object v6

    invoke-virtual {v5, v6}, Lcom/chad/library/adapter/base/BaseQuickAdapter;->oOO0(Landroid/view/View;)V

    .line 195
    iget v5, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O0O0:I

    if-ne v5, v3, :cond_889

    iget-boolean v3, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O00O:Z

    if-eqz v3, :cond_889

    .line 196
    iput-boolean v2, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O00O:Z

    .line 197
    sget-object v2, LO0oOo/O00O00;->O0Oo:Ljava/lang/String;

    .line 198
    invoke-static {v2}, LOOOOo/OO0O;->OO00(Ljava/lang/String;)LOOOOo/OO0O;

    move-result-object v2

    .line 199
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->O0OO()Lcom/caoliu/lib_common/base/BaseViewModel;

    move-result-object v3

    check-cast v3, Lcom/caoliu/module_im/chat/ChatViewModel;

    .line 200
    iget-object v7, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O0OO:Ljava/lang/String;

    .line 201
    iget-object v3, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O0o0:Lcom/caoliu/lib_common/entity/WebSocketResponse$Data$SentMemberInfo;

    if-eqz v3, :cond_853

    invoke-virtual {v3}, Lcom/caoliu/lib_common/entity/WebSocketResponse$Data$SentMemberInfo;->getMemberId()Ljava/lang/String;

    move-result-object v4

    :cond_853
    invoke-static {v4}, Ljava/lang/String;->valueOf(Ljava/lang/Object;)Ljava/lang/String;

    move-result-object v9

    .line 202
    iget-object v10, v1, Lcom/caoliu/module_im/chat/ChatNewActivity;->O0Oo:Ljava/lang/String;

    const-string v1, "dialogueId"

    .line 203
    invoke-static {v7, v1}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    const-string v1, "recvMemberId"

    invoke-static {v10, v1}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 204
    new-instance v1, Lcom/caoliu/module_im/entity/PriRequest;

    .line 205
    new-instance v3, Lcom/caoliu/module_im/entity/PriRequest$Data;

    .line 206
    sget-object v4, Lcom/caoliu/module_im/OOO0;->OOOO:Lcom/caoliu/module_im/OOOO;

    const/4 v8, 0x1

    const-string v6, "cls"

    move-object v5, v3

    .line 207
    invoke-direct/range {v5 .. v10}, Lcom/caoliu/module_im/entity/PriRequest$Data;-><init>(Ljava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;)V

    .line 208
    invoke-static {}, Ljava/lang/System;->currentTimeMillis()J

    move-result-wide v4

    const-string v6, "ESTABLISH_PRIVATE_CHAT_REQ"

    .line 209
    invoke-direct {v1, v6, v3, v4, v5}, Lcom/caoliu/module_im/entity/PriRequest;-><init>(Ljava/lang/String;Lcom/caoliu/module_im/entity/PriRequest$Data;J)V

    .line 210
    invoke-static {v1}, Lcom/blankj/utilcode/util/GsonUtils;->toJson(Ljava/lang/Object;)Ljava/lang/String;

    move-result-object v1

    const-string v3, "toJson(json)"

    invoke-static {v1, v3}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    .line 211
    iget-object v2, v2, LOOOOo/OO0O;->OOoO:Lokhttp3/OOOOO0;

    if-eqz v2, :cond_889

    .line 212
    invoke-interface {v2, v1}, Lokhttp3/OOOOO0;->OOOO(Ljava/lang/String;)Z

    :cond_889
    return-void

    .line 213
    :pswitch_88a  #0x9
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/rive/runtime/module_pa/PaFragment;

    move-object/from16 v2, p1

    check-cast v2, Ljava/util/List;

    sget v4, Lapp/rive/runtime/module_pa/PaFragment;->O0O0:I

    .line 214
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 215
    new-instance v4, Lcom/caoliu/lib_common/entity/MediaLabelResponse;

    move-object v13, v4

    const/4 v14, 0x0

    const/4 v15, 0x0

    const/16 v16, 0x0

    const/16 v17, 0x0

    const/16 v18, 0x0

    const/16 v19, 0x0

    const/16 v20, 0x0

    const/16 v21, 0x0

    const/16 v22, 0x0

    const/16 v23, 0x0

    const/16 v24, 0x0

    const/16 v25, 0x0

    const/16 v28, 0x0

    const/16 v29, 0x0

    const/16 v30, 0x0

    const/16 v31, 0x0

    const/16 v32, 0x0

    const/16 v33, 0x0

    const v34, 0xfcfff

    const/16 v35, 0x0

    const-string v26, ""

    const-string v27, "我喜欢的"

    invoke-direct/range {v13 .. v35}, Lcom/caoliu/lib_common/entity/MediaLabelResponse;-><init>(Lcom/caoliu/lib_common/entity/BannerBean;Ljava/lang/String;IILjava/lang/String;Ljava/lang/String;Ljava/lang/String;IILjava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;Ljava/lang/String;IZILkotlin/jvm/internal/OOO00;)V

    invoke-interface {v2, v4}, Ljava/util/List;->add(Ljava/lang/Object;)Z

    .line 216
    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v4

    if-lez v4, :cond_8e0

    .line 217
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;

    iget-object v4, v4, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;->OooO:Landroidx/viewpager2/widget/ViewPager2;

    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v5

    invoke-virtual {v4, v5}, Landroidx/viewpager2/widget/ViewPager2;->setOffscreenPageLimit(I)V

    .line 218
    :cond_8e0
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;

    iget-object v4, v4, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;->OooO:Landroidx/viewpager2/widget/ViewPager2;

    invoke-virtual {v1}, Landroidx/fragment/app/Fragment;->getChildFragmentManager()Landroidx/fragment/app/FragmentManager;

    move-result-object v5

    invoke-virtual {v1}, Landroidx/fragment/app/Fragment;->getLifecycle()Landroidx/lifecycle/Lifecycle;

    move-result-object v6

    new-instance v7, Lapp/rive/runtime/module_pa/PaFragment$startObserve$2$1;

    invoke-direct {v7, v2, v5, v6}, Lapp/rive/runtime/module_pa/PaFragment$startObserve$2$1;-><init>(Ljava/util/List;Landroidx/fragment/app/FragmentManager;Landroidx/lifecycle/Lifecycle;)V

    invoke-virtual {v4, v7}, Landroidx/viewpager2/widget/ViewPager2;->setAdapter(Landroidx/recyclerview/widget/RecyclerView$Adapter;)V

    .line 219
    new-instance v4, Lcom/google/android/material/tabs/TabLayoutMediator;

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;

    iget-object v5, v5, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;->OoOo:Lcom/google/android/material/tabs/TabLayout;

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;

    iget-object v1, v1, Lapp/rive/runtime/module_pa/databinding/FragmentPaBinding;->OooO:Landroidx/viewpager2/widget/ViewPager2;

    .line 220
    new-instance v6, Lapp/a/module_comic/fragment/OO0O;

    invoke-direct {v6, v2, v3}, Lapp/a/module_comic/fragment/OO0O;-><init>(Ljava/util/List;I)V

    .line 221
    invoke-direct {v4, v5, v1, v6}, Lcom/google/android/material/tabs/TabLayoutMediator;-><init>(Lcom/google/android/material/tabs/TabLayout;Landroidx/viewpager2/widget/ViewPager2;Lcom/google/android/material/tabs/TabLayoutMediator$TabConfigurationStrategy;)V

    .line 222
    invoke-virtual {v4}, Lcom/google/android/material/tabs/TabLayoutMediator;->attach()V

    return-void

    .line 223
    :pswitch_916  #0x8
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/fragment/ReaderListFragment;

    move-object/from16 v2, p1

    check-cast v2, Ljava/util/List;

    sget-object v3, Lapp/a/module_comic/fragment/ReaderListFragment;->oOOo:Lapp/a/module_comic/fragment/ReaderListFragment$OOOO;

    .line 224
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 225
    iget-object v3, v1, Lapp/a/module_comic/fragment/ReaderListFragment;->O000:Ljava/util/ArrayList;

    invoke-virtual {v3}, Ljava/util/ArrayList;->clear()V

    .line 226
    invoke-interface {v2}, Ljava/util/List;->size()I

    move-result v3

    if-lez v3, :cond_933

    .line 227
    iget-object v3, v1, Lapp/a/module_comic/fragment/ReaderListFragment;->O000:Ljava/util/ArrayList;

    invoke-virtual {v3, v2}, Ljava/util/ArrayList;->addAll(Ljava/util/Collection;)Z

    .line 228
    :cond_933
    invoke-virtual {v1}, Lapp/a/module_comic/fragment/ReaderListFragment;->O0oo()V

    return-void

    .line 229
    :pswitch_937  #0x7
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/fragment/ComicListFragment;

    move-object/from16 v4, p1

    check-cast v4, Lcom/caoliu/lib_http/PageData;

    sget-object v5, Lapp/a/module_comic/fragment/ComicListFragment;->oOOO:Lapp/a/module_comic/fragment/ComicListFragment$OOOO;

    .line 230
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 231
    invoke-static {}, Lcom/blankj/utilcode/util/SPUtils;->getInstance()Lcom/blankj/utilcode/util/SPUtils;

    move-result-object v5

    const/16 v7, 0x14

    const-string v8, "inADNub"

    invoke-virtual {v5, v8, v7}, Lcom/blankj/utilcode/util/SPUtils;->getInt(Ljava/lang/String;I)I

    move-result v5

    .line 232
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v7

    check-cast v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v7, v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oooo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v4}, Lcom/caoliu/lib_http/PageData;->getDataList()Ljava/util/ArrayList;

    move-result-object v8

    invoke-virtual {v8}, Ljava/util/ArrayList;->size()I

    move-result v8

    if-le v5, v8, :cond_964

    const/4 v8, 0x1

    goto :goto_965

    :cond_964
    const/4 v8, 0x0

    :goto_965
    invoke-virtual {v7, v2, v3, v8}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OoO0(IZZ)Lo0o0O/O0O00;

    .line 233
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v7

    check-cast v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v7, v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oooo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v4}, Lcom/caoliu/lib_http/PageData;->getDataList()Ljava/util/ArrayList;

    move-result-object v8

    invoke-virtual {v8}, Ljava/util/ArrayList;->size()I

    move-result v8

    if-le v5, v8, :cond_97c

    const/4 v8, 0x1

    goto :goto_97d

    :cond_97c
    const/4 v8, 0x0

    :goto_97d
    invoke-virtual {v7, v8}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->O0oo(Z)Lo0o0O/O0O00;

    .line 234
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v7

    check-cast v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v7, v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oooo:Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;

    invoke-virtual {v7}, Lcom/scwang/smart/refresh/layout/SmartRefreshLayout;->OOOO()Lo0o0O/O0O00;

    .line 235
    iget v7, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0OO:I

    const-string v8, "mBinding.rv"

    if-ne v7, v3, :cond_9a4

    .line 236
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v6

    check-cast v6, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v6, v6, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo0o:Landroidx/recyclerview/widget/RecyclerView;

    invoke-static {v6, v8}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-virtual {v4}, Lcom/caoliu/lib_http/PageData;->getDataList()Ljava/util/ArrayList;

    move-result-object v4

    invoke-static {v6, v4}, LO0oOo/O00O00;->OoO0(Landroidx/recyclerview/widget/RecyclerView;Ljava/util/List;)V

    goto :goto_9b6

    .line 237
    :cond_9a4
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v7

    check-cast v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v7, v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo0o:Landroidx/recyclerview/widget/RecyclerView;

    invoke-static {v7, v8}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-virtual {v4}, Lcom/caoliu/lib_http/PageData;->getDataList()Ljava/util/ArrayList;

    move-result-object v4

    invoke-static {v7, v4, v2, v2, v6}, LO0oOo/O00O00;->OOo0(Landroidx/recyclerview/widget/RecyclerView;Ljava/util/List;ZII)V

    .line 238
    :goto_9b6
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v4, v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo0o:Landroidx/recyclerview/widget/RecyclerView;

    invoke-static {v4, v8}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-static {v4}, LO0oOo/O00O00;->OO00(Landroidx/recyclerview/widget/RecyclerView;)Ljava/util/ArrayList;

    move-result-object v4

    invoke-virtual {v4}, Ljava/util/ArrayList;->size()I

    move-result v4

    if-nez v4, :cond_9d7

    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v4, v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo00:Landroid/view/View;

    invoke-virtual {v4, v2}, Landroid/view/View;->setVisibility(I)V

    goto :goto_9e4

    .line 239
    :cond_9d7
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v4

    check-cast v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v4, v4, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo00:Landroid/view/View;

    const/16 v6, 0x8

    invoke-virtual {v4, v6}, Landroid/view/View;->setVisibility(I)V

    .line 240
    :goto_9e4
    iget-object v4, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0o0:Ljava/util/ArrayList;

    invoke-virtual {v4}, Ljava/util/ArrayList;->size()I

    move-result v4

    if-ge v4, v3, :cond_9ee

    goto/16 :goto_a6e

    :cond_9ee
    add-int/2addr v5, v3

    .line 241
    iget v4, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oo:I

    :goto_9f1
    add-int/2addr v4, v3

    mul-int v4, v4, v5

    sub-int/2addr v4, v3

    .line 242
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v6

    check-cast v6, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v6, v6, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo0o:Landroidx/recyclerview/widget/RecyclerView;

    invoke-static {v6, v8}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-static {v6}, LO0oOo/O00O00;->OO0o(Landroidx/recyclerview/widget/RecyclerView;)Lcom/drake/brv/BindingAdapter;

    move-result-object v6

    invoke-virtual {v6}, Lcom/drake/brv/BindingAdapter;->OOoo()I

    move-result v6

    if-gt v4, v6, :cond_a6e

    .line 243
    iget-object v6, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0o0:Ljava/util/ArrayList;

    invoke-virtual {v6}, Ljava/util/ArrayList;->size()I

    move-result v6

    iget v7, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oO:I

    if-lt v6, v7, :cond_a16

    iput v2, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oO:I

    .line 244
    :cond_a16
    new-instance v6, Ljava/util/ArrayList;

    invoke-direct {v6}, Ljava/util/ArrayList;-><init>()V

    .line 245
    new-instance v7, Lcom/caoliu/lib_common/entity/MediaLabelResponse;

    move-object v10, v7

    iget-object v11, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0o0:Ljava/util/ArrayList;

    iget v12, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oO:I

    invoke-virtual {v11, v12}, Ljava/util/ArrayList;->get(I)Ljava/lang/Object;

    move-result-object v11

    check-cast v11, Lcom/caoliu/lib_common/entity/BannerBean;

    const/4 v12, 0x0

    const/4 v13, 0x0

    const/4 v14, 0x0

    const/4 v15, 0x0

    const/16 v16, 0x0

    const/16 v17, 0x0

    const/16 v19, 0x0

    move/from16 v18, v19

    const/16 v20, 0x0

    const/16 v21, 0x0

    const/16 v22, 0x0

    const/16 v23, 0x0

    const/16 v24, 0x0

    const/16 v25, 0x0

    const/16 v26, 0x0

    const/16 v27, 0x0

    const/16 v28, 0x0

    const/16 v29, 0x0

    const/16 v30, 0x0

    const v31, 0xffffe

    const/16 v32, 0x0

    invoke-direct/range {v10 .. v32}, Lcom/caoliu/lib_common/entity/MediaLabelResponse;-><init>(Lcom/caoliu/lib_common/entity/BannerBean;Ljava/lang/String;IILjava/lang/String;Ljava/lang/String;Ljava/lang/String;IILjava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;Ljava/lang/String;IZILkotlin/jvm/internal/OOO00;)V

    .line 246
    invoke-virtual {v6, v7}, Ljava/util/ArrayList;->add(Ljava/lang/Object;)Z

    .line 247
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->OO0o()Landroidx/databinding/ViewDataBinding;

    move-result-object v7

    check-cast v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;

    iget-object v7, v7, Lapp/a/module_comic/databinding/FragmentComicListBinding;->Oo0o:Landroidx/recyclerview/widget/RecyclerView;

    invoke-static {v7, v8}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-static {v7, v6, v2, v4, v9}, LO0oOo/O00O00;->OOo0(Landroidx/recyclerview/widget/RecyclerView;Ljava/util/List;ZII)V

    .line 248
    iget v4, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oo:I

    add-int/2addr v4, v3

    iput v4, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oo:I

    .line 249
    iget v6, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oO:I

    add-int/2addr v6, v3

    iput v6, v1, Lapp/a/module_comic/fragment/ComicListFragment;->O0oO:I

    goto :goto_9f1

    :cond_a6e
    :goto_a6e
    return-void

    .line 250
    :pswitch_a6f  #0x6
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/fragment/ComicHomeFragment;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lapp/a/module_comic/fragment/ComicHomeFragment;->O0oo:I

    .line 251
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 252
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseFragment;->Oo0o(Z)V

    return-void

    .line 253
    :pswitch_a84  #0x5
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/ComicDetailActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/entity/ComicDetailResponse;

    invoke-static {v1, v2}, Lapp/a/module_comic/ComicDetailActivity;->O00o(Lapp/a/module_comic/ComicDetailActivity;Lcom/caoliu/lib_common/entity/ComicDetailResponse;)V

    return-void

    :pswitch_a90  #0x4
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/ComicActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;

    sget v5, Lapp/a/module_comic/ComicActivity;->O0oo:I

    .line 254
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 255
    iput-object v2, v1, Lapp/a/module_comic/ComicActivity;->Oo00:Lcom/caoliu/lib_common/entity/ComicResponse$Comic;

    .line 256
    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    .line 257
    invoke-virtual {v1}, Lapp/a/module_comic/ComicActivity;->O00o()V

    .line 258
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lapp/a/module_comic/databinding/ActivityComicBinding;

    iget-object v12, v5, Lapp/a/module_comic/databinding/ActivityComicBinding;->OooO:Landroid/widget/ImageView;

    const-string v5, "mBinding.img"

    invoke-static {v12, v5}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;->getComicVo()Lcom/caoliu/lib_common/entity/ComicResponse$ComicVo;

    move-result-object v5

    if-eqz v5, :cond_abe

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ComicResponse$ComicVo;->getComicCover()Ljava/lang/String;

    move-result-object v5

    move-object v13, v5

    goto :goto_abf

    :cond_abe
    move-object v13, v4

    :goto_abf
    const/4 v14, 0x0

    const/4 v15, 0x0

    const/16 v16, 0x0

    const/16 v17, 0xe

    invoke-static/range {v12 .. v17}, Lcom/caoliu/lib_common/ExKt;->O000(Landroid/widget/ImageView;Ljava/lang/String;IIII)V

    .line 259
    invoke-virtual {v1}, Lapp/a/module_comic/ComicActivity;->oOOO()V

    .line 260
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v5

    check-cast v5, Lapp/a/module_comic/databinding/ActivityComicBinding;

    iget-object v5, v5, Lapp/a/module_comic/databinding/ActivityComicBinding;->O0O0:Landroid/widget/TextView;

    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;->getComicVo()Lcom/caoliu/lib_common/entity/ComicResponse$ComicVo;

    move-result-object v6

    if-eqz v6, :cond_add

    invoke-virtual {v6}, Lcom/caoliu/lib_common/entity/ComicResponse$ComicVo;->getComicName()Ljava/lang/String;

    move-result-object v4

    :cond_add
    invoke-virtual {v5, v4}, Landroid/widget/TextView;->setText(Ljava/lang/CharSequence;)V

    .line 261
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;->getTagList()Ljava/util/List;

    move-result-object v4

    invoke-interface {v4}, Ljava/util/Collection;->isEmpty()Z

    move-result v4

    xor-int/2addr v3, v4

    if-eqz v3, :cond_b37

    .line 262
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v3

    check-cast v3, Lapp/a/module_comic/databinding/ActivityComicBinding;

    iget-object v3, v3, Lapp/a/module_comic/databinding/ActivityComicBinding;->OoO0:Lcom/caoliu/lib_common/widget/FlowLayout;

    invoke-virtual {v3}, Landroid/widget/RelativeLayout;->removeAllViews()V

    .line 263
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;->getTagList()Ljava/util/List;

    move-result-object v3

    invoke-static {v3}, LO0oOo/O00OO0;->oO00(Ljava/util/Collection;)LOOO0oo/OOO0OO;

    move-result-object v3

    .line 264
    new-instance v4, Ljava/util/ArrayList;

    invoke-static {v3, v11}, Lkotlin/collections/OO00O;->OO0oO(Ljava/lang/Iterable;I)I

    move-result v5

    invoke-direct {v4, v5}, Ljava/util/ArrayList;-><init>(I)V

    .line 265
    invoke-virtual {v3}, LOOO0oo/OOOO0O;->OOOO()Lkotlin/collections/O0000;

    move-result-object v3

    .line 266
    :goto_b0b
    move-object v5, v3

    check-cast v5, LOOO0oo/OOOO00;

    .line 267
    iget-boolean v5, v5, LOOO0oo/OOOO00;->OooO:Z

    if-eqz v5, :cond_b2c

    .line 268
    invoke-virtual {v3}, Lkotlin/collections/O0000;->nextInt()I

    move-result v5

    .line 269
    invoke-virtual {v2}, Lcom/caoliu/lib_common/entity/ComicResponse$Comic;->getTagList()Ljava/util/List;

    move-result-object v6

    invoke-interface {v6, v5}, Ljava/util/List;->get(I)Ljava/lang/Object;

    move-result-object v5

    check-cast v5, Lcom/caoliu/lib_common/entity/ComicResponse$Tag;

    invoke-virtual {v5}, Lcom/caoliu/lib_common/entity/ComicResponse$Tag;->getTagName()Ljava/lang/String;

    move-result-object v5

    invoke-static {v1, v5}, Lcom/caoliu/lib_common/dialog/ShareDynamicDialogKt;->OOOO(Landroid/content/Context;Ljava/lang/String;)Landroid/view/View;

    move-result-object v5

    invoke-virtual {v4, v5}, Ljava/util/ArrayList;->add(Ljava/lang/Object;)Z

    goto :goto_b0b

    .line 270
    :cond_b2c
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseActivity;->Oo00()Landroidx/databinding/ViewDataBinding;

    move-result-object v1

    check-cast v1, Lapp/a/module_comic/databinding/ActivityComicBinding;

    iget-object v1, v1, Lapp/a/module_comic/databinding/ActivityComicBinding;->OoO0:Lcom/caoliu/lib_common/widget/FlowLayout;

    invoke-virtual {v1, v4}, Lcom/caoliu/lib_common/widget/FlowLayout;->setChildren(Ljava/util/ArrayList;)V

    :cond_b37
    return-void

    .line 271
    :pswitch_b38  #0x3
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_comic/ArticleActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lapp/a/module_comic/ArticleActivity;->Oo00:I

    .line 272
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 273
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    return-void

    .line 274
    :pswitch_b4d  #0x2
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_ai/fragment/AiDiyFragment;

    move-object/from16 v15, p1

    check-cast v15, Ljava/lang/String;

    sget v3, Lapp/a/module_ai/fragment/AiDiyFragment;->O000:I

    .line 275
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 276
    invoke-static {v15}, Landroid/text/TextUtils;->isEmpty(Ljava/lang/CharSequence;)Z

    move-result v3

    if-eqz v3, :cond_b6d

    .line 277
    iput-boolean v2, v1, Lapp/a/module_ai/fragment/AiDiyFragment;->O00O:Z

    .line 278
    iget-object v3, v1, Lcom/caoliu/lib_common/base/BaseFragment;->Oo0o:Lcom/caoliu/lib_common/dialog/OOO00;

    if-eqz v3, :cond_b69

    .line 279
    invoke-virtual {v3, v7}, Lcom/caoliu/lib_common/dialog/OOO00;->OO0O(Ljava/lang/String;)V

    .line 280
    :cond_b69
    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseFragment;->Oo0o(Z)V

    goto :goto_b96

    .line 281
    :cond_b6d
    iget-object v2, v1, Lcom/caoliu/lib_common/base/BaseFragment;->Oo0o:Lcom/caoliu/lib_common/dialog/OOO00;

    if-eqz v2, :cond_b76

    const-string v3, "制作中..."

    .line 282
    invoke-virtual {v2, v3}, Lcom/caoliu/lib_common/dialog/OOO00;->OO0O(Ljava/lang/String;)V

    .line 283
    :cond_b76
    invoke-virtual {v1}, Lcom/caoliu/lib_common/base/BaseFragment;->Oooo()Lcom/caoliu/lib_common/base/BaseViewModel;

    move-result-object v2

    move-object v13, v2

    check-cast v13, Lapp/a/module_ai/AIViewModel;

    .line 284
    invoke-virtual {v1}, Landroidx/fragment/app/Fragment;->requireContext()Landroid/content/Context;

    move-result-object v14

    const-string v2, "requireContext()"

    invoke-static {v14, v2}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    .line 285
    invoke-static {v15, v10}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    const/16 v17, 0x1

    .line 286
    iget-object v1, v1, Lapp/a/module_ai/fragment/AiDiyFragment;->O00o:Ljava/lang/String;

    const-string v16, ""

    const-string v18, ""

    move-object/from16 v19, v1

    .line 287
    invoke-virtual/range {v13 .. v19}, Lapp/a/module_ai/AIViewModel;->OoOo(Landroid/content/Context;Ljava/lang/String;Ljava/lang/String;ILjava/lang/String;Ljava/lang/String;)V

    :goto_b96
    return-void

    .line 288
    :pswitch_b97  #0x1
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_ai/fragment/AiClearFragment;

    move-object/from16 v3, p1

    check-cast v3, Ljava/lang/Boolean;

    sget v5, Lapp/a/module_ai/fragment/AiClearFragment;->oOOO:I

    .line 289
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 290
    iput-boolean v2, v1, Lapp/a/module_ai/fragment/AiClearFragment;->O00o:Z

    .line 291
    invoke-static {v3, v10}, Lkotlin/jvm/internal/OO0O0;->OOoo(Ljava/lang/Object;Ljava/lang/String;)V

    invoke-virtual {v3}, Ljava/lang/Boolean;->booleanValue()Z

    move-result v2

    if-eqz v2, :cond_bd1

    const-string v2, "上传成功"

    .line 292
    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseFragment;->O0OO(Ljava/lang/String;)V

    .line 293
    iget v2, v1, Lapp/a/module_ai/fragment/AiClearFragment;->O0O0:I

    invoke-virtual {v1, v2}, Lapp/a/module_ai/fragment/AiClearFragment;->O0O0(I)V

    .line 294
    invoke-static {}, Lcom/blankj/utilcode/util/SPUtils;->getInstance()Lcom/blankj/utilcode/util/SPUtils;

    move-result-object v2

    invoke-static {}, Ljava/lang/System;->currentTimeMillis()J

    move-result-wide v5

    const-string v3, "upload_time"

    invoke-virtual {v2, v3, v5, v6}, Lcom/blankj/utilcode/util/SPUtils;->put(Ljava/lang/String;J)V

    const-string v2, "/ai/AiListActivity"

    .line 295
    invoke-static {v2, v4}, Lcom/caoliu/lib_common/ExKt;->O0oo(Ljava/lang/String;LOOO0Oo/OO0OO;)V

    .line 296
    iget v2, v1, Lapp/a/module_ai/fragment/AiClearFragment;->O0OO:I

    invoke-virtual {v1, v2}, Lapp/a/module_ai/fragment/AiClearFragment;->O0O0(I)V

    goto :goto_bd6

    .line 297
    :cond_bd1
    iget v2, v1, Lapp/a/module_ai/fragment/AiClearFragment;->O0Oo:I

    invoke-virtual {v1, v2}, Lapp/a/module_ai/fragment/AiClearFragment;->O0O0(I)V

    :goto_bd6
    return-void

    .line 298
    :pswitch_bd7  #0x0
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lapp/a/module_ai/AiListItemFragment;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lapp/a/module_ai/AiListItemFragment;->O0oo:I

    .line 299
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 300
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseFragment;->Oo0o(Z)V

    return-void

    .line 301
    :goto_bec
    iget-object v1, v0, Lapp/a/module_ai/O0OO;->OOOo:Ljava/lang/Object;

    check-cast v1, Lcom/caoliu/module_mine/question/QuestionListDetailActivity;

    move-object/from16 v2, p1

    check-cast v2, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;

    sget v3, Lcom/caoliu/module_mine/question/QuestionListDetailActivity;->Oo00:I

    .line 302
    invoke-static {v1, v12}, Lkotlin/jvm/internal/OO0O0;->OOo0(Ljava/lang/Object;Ljava/lang/String;)V

    .line 303
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getLoading()Z

    move-result v3

    invoke-virtual {v1, v3}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oO(Z)V

    .line 304
    invoke-virtual {v2}, Lcom/caoliu/lib_common/base/BaseViewModel$UiModel;->getShowMsg()Ljava/lang/String;

    move-result-object v2

    invoke-virtual {v1, v2}, Lcom/caoliu/lib_common/base/BaseActivity;->O0oo(Ljava/lang/String;)V

    return-void

    :pswitch_data_c08
    .packed-switch 0x0
        :pswitch_bd7  #00000000
        :pswitch_b97  #00000001
        :pswitch_b4d  #00000002
        :pswitch_b38  #00000003
        :pswitch_a90  #00000004
        :pswitch_a84  #00000005
        :pswitch_a6f  #00000006
        :pswitch_937  #00000007
        :pswitch_916  #00000008
        :pswitch_88a  #00000009
        :pswitch_805  #0000000a
        :pswitch_7a6  #0000000b
        :pswitch_6d6  #0000000c
        :pswitch_6ba  #0000000d
        :pswitch_6a5  #0000000e
        :pswitch_603  #0000000f
        :pswitch_5ee  #00000010
        :pswitch_4b3  #00000011
        :pswitch_497  #00000012
        :pswitch_43d  #00000013
        :pswitch_38a  #00000014
        :pswitch_364  #00000015
        :pswitch_34f  #00000016
        :pswitch_247  #00000017
        :pswitch_1f5  #00000018
        :pswitch_c8  #00000019
        :pswitch_86  #0000001a
        :pswitch_73  #0000001b
        :pswitch_1a  #0000001c
    .end packed-switch
.end method
