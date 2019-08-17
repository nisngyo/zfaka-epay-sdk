# zfaka-epay-sdk

zfaka 的易支付接口

1.把Pay下面的 三个文件夹alpayalipay,alpaywxpay,alpayqqpay 上传到zfaka程序的application\library\Pay文件夹下

2.把tpl下面的三个文件 alpayalipay.html,alpaywxpay.html,alpayqqpay.html 上传到application\modules\Admin\views\payment\tpl 下面

3.进入数据库插入3条数据

 INSERT INTO `t_payment`( `payment`, `payname`, `payimage`, `alias`, `sign_type`) VALUES 
('易支付支付宝', '支付宝', '/res/images/pay/alipay.jpg', 'alpayalipay', 'MD5'),
('易支付微信', '微信支付', '/res/images/pay/weixin.jpg', 'alpaywxpay', 'MD5'),
('易支付QQ', 'QQ支付', '/res/images/pay/qqpay.jpg', 'alpayqqpay', 'MD5');

上面3步完成后就可以到后台设置支付接口了

