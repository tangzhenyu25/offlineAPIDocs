# 添加分账方
**简要描述：**
- 退费状态查询

**请求URL：** 
- 商户->联动优势
`{交易服务根地址}/merchants/ledgerAcqMerIdAdd`

**请求方式：**
- POST 

**请求参数：** 

|	字段	|	名称	|	长度	|	必填	|   说明|
|:--------:|:--------:|:--------:|:--------:|:--------|
|	acqSpId	|	代理商编号	|	10	|	M	|	代理商编号(联动平台分配)	|
|	acqMerId	|	商户号	|	8	|	M	|	商户号(联动平台分配)	|
|	ledgerAcqMerInfo	|	分账订单号	|	64	|	M	|	商户的分账支付订单号	|
|	signature	|	签名	|	256	|	M	|参见签名机制	|	|
|	|
|	ledgerAcqMerInfo格式如下：		|
|	字段	 |	名称	  |	长度  	|	必填  	|	说明	  |
|	ledgerAcqMerId	|	分账商户号	|	8	|	M	|		|



 **返回参数说明** 
 
|	字段	|	名称	|	长度	|	必填	|	说明	|
|--------|-------|--------|--------|--------|
|	respCode	|	返回码	|	8	|	M	|	返回码	|
|	respMsg	|	返回信息	|	128	|	M	|	返回信息	|