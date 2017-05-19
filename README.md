# xiaobao
## 大小
### 大小
#### 大小
##### 大小
###### 大小##大小
```
 public FundResult modifyStatus(@RequestParam(value = "userId") Integer userId,@RequestParam(value = "investPlanId") String investPlanId,
                                   @RequestParam(value = "opType") String opType) {
        FundInvestPlanOPType fundInvestPlanOPType = FundInvestPlanOPType.valOf(opType);
        CallbackResult<FundInvestPlanResult> result = baseFundInvestPlanService.modifyFundInvestPlanStatus(userId, investPlanId, fundInvestPlanOPType);
        if (result.isSuccess()) {
            return FundResult.buildJsonResultFromReesult(result);
        } else {
            return FundResult.buildErrorVo("修改基金定投状态失败。");
        }
    }
```
大标题
===
小标题
---

![baidu](https://ss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo_top_ca79a146.png)
