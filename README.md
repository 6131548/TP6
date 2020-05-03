# TP6
TP6框架

#跳转
composer require liliuwei/thinkphp-jump
 #开启session
# /app/middleware.php 添加
# \think\middleware\SessionInit::class
# 验证器
#try {
            $result = validate(Adminuser::class)
                ->batch(true)
                ->check($event);
        } catch (\Exception $e) {
            // 验证失败 输出错误信息
           return json(['code' => 0, 'msg' => $e->getMessage()]);
        }
          
 
