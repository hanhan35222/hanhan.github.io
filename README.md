# hanhan.github.io
703555655qq跳转
<!DOCTYPE html>
<html>
<head>
    <title>添加QQ好友</title>
    <meta charset="utf-8">
    <script>
        (function() {
            // 请在此处替换为你的QQ号
            var qqNumber = '703555655'; 

            var mobileLink = 'mqq://im/chat?chat_type=wpa&uin=' + qqNumber + '&version=1&src_type=web';
            var pcLink = 'tencent://AddContact/?fromId=45&fromSubId=1&subcmd=all&uin=' + qqNumber;

            // 判断设备并跳转
            if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
                window.location.href = mobileLink;
                // 如果唤起APP失败，备用提示
                setTimeout(function() {
                    alert('如果未自动跳转，请确保已安装手机QQ。或手动搜索QQ号：' + qqNumber + ' 添加。');
                }, 800);
            } else {
                window.location.href = pcLink;
            }
        })();
    </script>
</head>
<body>
    <p>正在跳转到QQ添加好友...</p>
</body>
</html>
