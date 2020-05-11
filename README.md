# -PUBG-
罗技G系列LGS驱动lua宏代码和罗技G-HUB驱动lua代码

罗技鼠标G502 | G403 | G400S | G500S | G903 | G903REPO | G502REPO系列都支持，只要能装蓝色的LGS驱动或者黑色的GHUB驱动就可以使用压枪宏

PUBG = {}
-------------------------------------------------- -------------------------------------------------- -------	
----------------------------------------------------------------------------------------------------------- 
PUBG.ZG = "9.99"   
PUBG.GameFPS = "90"	  
PUBG.BanBen = "10.6"     
--------------------------------------------------------------------------
----------------        罗技G系列鼠标侧键     ----------------------------
--------------------------------------------------------------------------
-- 罗技鼠标区第一组枪【使用方式，直接按罗技鼠标的侧键就可以开启压枪】
-- 罗技鼠标区第二组枪【键盘左下角的ALT+罗技鼠标侧键就可以开启第二组压枪，和第一组不冲突】
-- 罗技键盘区【G1 = 1 或 F1 = 1 仅限支持驱动的罗技键盘，按下键盘后用罗技鼠标可以开启压枪】
--------------------------------------------------------------------------
PUBG.logitechKeyNum_M416 = 5		-- 名称| M416|不支持连点| 7.62子弹 | 补偿器+直角握把+枪托 = 满配
PUBG.logitechKeyNum_AKM = 4			-- 名称| AKM |不支持连点| 7.62子弹 | 补偿器 = 满配
PUBG.logitechKeyNum_GROZA = nil		-- 名称|GROZA|不支持连点| 7.62子弹 | 补偿器 = 满配
PUBG.logitechKeyNum_G36C = nil		-- 名称| G36C|不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_AUG = 10		-- 名称| AUG |不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_UMP45 = 7		-- 名称|UMP45|不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_SCARL = nil		-- 名称|SCARL|不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_PP19 = 9		-- 名称|PP19 |不支持连点| 7.62子弹 | 补偿器 = 满配
PUBG.logitechKeyNum_VSS = nil		-- 名称|VSS  |不支持连点| 7.62子弹 | 补偿器+托腮板 = 满配
PUBG.logitechKeyNum_M762 = nil		-- 名称| M762|不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_M249 = nil		-- 名称| M249|不支持连点| 7.62子弹 | 枪托 = 满配
PUBG.logitechKeyNum_QBZ95 = nil		-- 名称|QBZ95|不支持连点| 7.62子弹 | 补偿器+直角握把 = 满配
PUBG.logitechKeyNum_M16A4 = 8		-- 名称|M16A4|支持有连点| 7.62子弹 | 补偿器+枪托 = 满配
PUBG.logitechKeyNum_SKS = 11		-- 名称| SKS |支持有连点| 7.62子弹 | 补偿器+直角握把+托腮板 = 满配
PUBG.logitechKeyNum_MINI14 = nil	-- 名称| Mini|支持有连点| 7.62子弹 | 补偿器 = 满配
PUBG.logitechKeyNum_LD = nil		-- 名称| 只连点 |不压枪 | 连点功能仅限在蓝色罗技驱动使用，黑色的G-HUB驱动不支持；	
PUBG.logitechKeyNum_GB = 6  		-- 名称|Close|关闭所有宏压枪|	
--------------------------------------------------------------------------
----------------        罗技第二组鼠标侧键     ---------------------------
--------------------------------------------------------------------------
-- 罗技鼠标区第二组枪【键盘左下角的ALT+罗技鼠标侧键就可以开启第二组压枪，和第一组不冲突】
--------------------------------------------------------------------------
PUBG.M416_control = nil
PUBG.AKM_control = nil
PUBG.GROZA_control = 10 
PUBG.G36C_control = 6
PUBG.AUG_control = nil
PUBG.UMP45_control = nil
PUBG.SCARL_control = nil
PUBG.PP19_control = nil
PUBG.VSS_control = 7
PUBG.M762_control = 4
PUBG.M249_control = 9
PUBG.QBZ95_control = 5
PUBG.M16A4_control = nil
PUBG.SKS_control = nil
PUBG.MINI14_control = 8
PUBG.LD_control = nil	
PUBG.GB_control = nil
--------------------------------------------------------------------------
----------------        罗技G系列键盘按键     ----------------------------
--------------------------------------------------------------------------
-- 罗技键盘区【G1 = 1 或 F1 = 1 仅限支持驱动的罗技键盘，按下键盘后用罗技鼠标可以开启压枪】
--------------------------------------------------------------------------
PUBG.M416_gkey = nil
PUBG.AKM_gkey = nil
PUBG.GROZA_gkey = nil
PUBG.G36C_gkey = 6
PUBG.AUG_gkey = nil
PUBG.UMP45_gkey = nil
PUBG.SCARL_gkey = nil
PUBG.PP19_gkey = nil
PUBG.VSS_gkey = nil
PUBG.M762_gkey = 4
PUBG.M249_gkey = nil
PUBG.QBZ95_gkey = 5
PUBG.M16A4_gkey = nil
PUBG.SKS_gkey = nil
PUBG.MINI14_gkey = nil
PUBG.LD_gkey = nil	
PUBG.GB_gkey = nil
--------------------------------------------------------------------------
----------------           辅助型功能开关     ----------------------------
--------------------------------------------------------------------------
-- 侧键编号 | 默认关闭 改为true时，你按侧键时会在脚本下方面板显示你当前按的侧键编号数字
PUBG.CeJian = false	
-- 连点功能 | 设置为false所有武器都有连点功能，设置为true仅M16、SKS、Mini会连点，而且不支持G-HUB驱动[G-HUB 驱动不要动这个]
PUBG.Auto_Mode = true
-- 快速开镜 | 默认关闭 改为true时，左键舔包不下压（压枪方式:先按住鼠标右键再按左键啊啊）
PUBG.quickfire = true	
-- 重复关宏 | 默认关闭 改为true时，同一个侧键按第二次关闭宏
PUBG.ERGB = false	
-- 满配功能 | 满配模式开关(不要满配模式就设置为false)
PUBG.Full_Mode = true
-- 四倍功能 | 四倍模式开关(不要四倍模式就设置为false)
PUBG.Full_Mode4X = true
-- 屏息功能 | 屏息模式开关(不要屏息模式就设置为false)
PUBG.Shift_Mode = true
-- 蹲下功能 | 蹲下模式开关(不要蹲下模式就设置为false)
PUBG.Ctrl_Mode = true
-- 自动换蛋（连续打完40发子弹自动换子弹的）
PUBG.ZDHD = true
--------------------------------------------------------------------------
----------------        一键拖拽物品功能设置     -------------------------
--------------------------------------------------------------------------
-- 拖拽物品 | 设置鼠标侧键快速拖拽物品（默认按一下拖拽3次，下面可修改拖拽次数）
PUBG.YJDcSq = 0 
-- 拖拽次数 | 按一下侧键后下方设置拖拽几次它就几次
PUBG.SqCshu = 3   
-- 拖拽方向 | 拖拽向右移动，修改此值可能会影响拖拽不能装上配件的啊
PUBG.Move = 40    
-- 拖拽方向 | 拖拽向上移动，修改此值可能会拖拽时漏掉物品啊
PUBG.Moveup = 60 
-- 拖拽物品 | 设置鼠标侧键一键拖拽物品，按一下拖拽一次（这个是备用的）
PUBG.YJDcSq2 = 0
-------------------------------------------------------------------------- 
----------------           无影手功能设置（主用）     --------------------
--------------------------------------------------------------------------
-- 宽屏设置 | 默认为1920*1080，设置为2 ： 2560*1080 设置为3 ：2560*1440 一般默认的分辨率即可啊
PUBG.Ping = "1"
-- 鬼手设置 | 设置一键拾取鬼手的鼠标侧键,设置按键(支持G系列鼠标和键盘)
PUBG.WYS = 0 
-- 宽屏调整 | 默认为设置好的，若在一键拾取时捡不起来物品，可向左(改成 -100 依次减少)或向右就相反 100 微调
PUBG.XY = 0 	 	
-- 自动装蛋 | 默认开启 改为false时，拾取武器自动装上弹夹就不给你装蛋了，默认打开不要关闭它
PUBG.ZDZT = true 
--------------------------------------------------------------------------
----------------           无影手功能设置（备用）     --------------------
--------------------------------------------------------------------------
-- 宽屏设置 | 默认为1920*1080，设置为2 ： 2560*1080 设置为3 ：2560*1440 一般默认的分辨率即可啊
PUBG.LZB_Ping = "1"
-- 鬼手设置 | 设置一键拾取鬼手的鼠标侧键,设置按键(支持G系列鼠标和键盘)--这个是备用的 来源ZY方法
PUBG.WYS2 = 0 
-- 鬼手装蛋 | 一键拾取物品时自动开背包，默认打开不要关闭它啊
PUBG.LZB_ZiDongKaiBeiBao = true 
-- 鬼手装蛋 | 一键拾取物品后自动装蛋，默认打开不要关闭它
PUBG.LZB_ZiDongHuanDan = true 
-- 持续拉拽 | 按下按键后不松开会持续拉拽（默认关闭 false）
PUBG.LZB_YiZhiLa = false 
--------------------------------------------------------------------------
----------------           新添加辅助功能     ----------------------------	
--------------------------------------------------------------------------
-- 切换手雷 | 设置侧键一键手雷，按一下就侧键就可以切换到手雷了（切记，按一下就扔一次 按10下就扔10次）
PUBG.YJSL = 0
-- 切换武器 | 扔出雷后自动切换主武器（1 就是主武器 这个不需要设置默认就好）
PUBG.SLYW = "1"
-- 一键横车 | 设置侧键一键横车，按一下侧键就可以横车（这个不是说你车都四脚朝天了还能给你翻过来，这个只是在翻滚时可以帮助你横车）
PUBG.YJHC = 0
-- 一键调窗 | 设置侧键一键跳窗，当你靠近窗户的时候，按一下侧键就可以从窗户跳出去
PUBG.YJTC = 0
-- 跳窗设置 | 跳窗的蹲改键开关 如果你的蹲改成了Ctrl键请打开这个开关（设为true）， 如果默认C键就改为false的啊啊啊
PUBG.TCGJ = false
--------------------------------------------------------------------------
----------------           热键区键盘设置     ------------------------------
--------------------------------------------------------------------------
-- 二组武器 | 切换第二组鼠标侧键时,按住键盘左下角的 Ctrl键+鼠标侧键
PUBG.D2Wq = "lalt" 
-- 临时关闭 | 按住此键可以临时关闭左键压枪，松开恢复压枪
PUBG.ignore_key = "lalt" 
-- 蹲下按键 | 蹲下时要按住左下角键盘的 Ctrl 键盘
PUBG.CTRL = "lctrl"
-- 屏息按键 | 屏息时要按住左下角键盘的 Shift 键盘
PUBG.Shift = "lshift"
-- 满配按键 | 开启/关闭满配的键盘按钮 		
PUBG.Full_Mode_key = "Numlock"   
-- 四倍按键 | 开启/关闭4倍的键盘按钮
PUBG.Mode_Switch_key = "Capslock" 
-- 灯光按键 | 这个是键盘指示灯,展示宏是否开启（灯亮是宏已经开启，灭就是没开启）
PUBG.Lighton_key = "Scrolllock" 
-- 肩射按键 | 肩射功能开关(按住鼠标右键可将四倍模式临时切换成红点模式)
PUBG.JianShe = true		
-- 满配反转 | 默认满配反转开启，空配模式与满配模式开启灯光反转（false =  灯亮满配  改为 true = 灯亮为空配）
PUBG.Full = true
--------------------------------------------------------------------------
----------------          武器系数强度调节    ------------------------------ 	
--------------------------------------------------------------------------
-- 设置屏幕 | 当前默认的是ping = "1080",如果你是2K屏，可以把ping = "1440",如果没有1080的稳，就改回来；
PUBG.PingMu = "1080" 
-- 压枪强度 | 这个是基础单倍压枪总系数，调整此值会影响所有的武器，谨慎调整；
PUBG.FenBianLv = 1.00
-- 压枪强度 | 这个是四倍模式压枪总系数，调整此值会影响所有的武器，谨慎调整；
PUBG.FenBianLv4X = 1.00
--------------------------------------------------------------------------
----- 站、蹲、屏息压不住，请把系数强度改大，压过头的话就改小	-------------------
--------------------------------------------------------------------------
PUBG.akm = 1.42       	--空配站着
PUBG.akmbx = 1.89     	--空配屏息
PUBG.akmdx = 1.05     	--空配蹲下
PUBG.akmal = 1.42      --满配站着
PUBG.akmalbx = 1.93   	--满配屏息
PUBG.akmaldx = 1.16   	--满配蹲下
PUBG.akm4x = 3.45   	--空配4倍站
PUBG.akm4xdx = 2.65   	--空配4倍蹲
PUBG.akmal4x = 3.65	--满配4倍站
PUBG.akmal4xdx = 2.80	--满配4倍蹲

PUBG.groza = 1.13       --空配站着
PUBG.grozabx = 1.50     --空配屏息
PUBG.grozadx = 0.85     --空配蹲下
PUBG.grozaal = 1.13     --满配站着
PUBG.grozaalbx = 1.50   --满配屏息
PUBG.grozaaldx = 0.85   --满配蹲下
PUBG.groza4x = 2.89     --空配4倍站
PUBG.groza4xdx = 2.00   --空配4倍蹲
PUBG.grozaal4x = 2.89   --满配4倍站
PUBG.grozaal4xdx = 2.00 --满配4倍蹲

PUBG.m762 = 1.62       --空配站着
PUBG.m762bx = 2.15     --空配屏息
PUBG.m762dx = 1.35     --空配蹲下
PUBG.m762al = 1.31     --满配站着
PUBG.m762albx = 1.70	--满配屏息
PUBG.m762aldx = 1.10   --满配蹲下
PUBG.m7624x = 4.20		--空配4倍站
PUBG.m7624xdx = 3.50   --空配4倍蹲
PUBG.m762al4x = 3.35	--满配4倍站
PUBG.m762al4xdx = 2.80 --满配4倍蹲

PUBG.m249 = 0.72       --空配站着
PUBG.m249bx = 0.97     --空配屏息
PUBG.m249dx = 0.47     --空配蹲下
PUBG.m249al = 0.72     --满配站着
PUBG.m249albx = 0.97   --满配屏息
PUBG.m249aldx = 0.47   --满配蹲下
PUBG.m2494x = 1.65     --空配4倍站
PUBG.m2494xdx = 0.90   --空配4倍蹲
PUBG.m249al4x = 1.81   --满配4倍站
PUBG.m249al4xdx = 0.98 --满配4倍蹲

PUBG.m16a4 = 1.20       --空配站着
PUBG.m16a4bx = 1.45     --空配屏息
PUBG.m16a4dx = 0.90     --空配蹲下
PUBG.m16a4al = 0.97     --满配站着
PUBG.m16a4albx = 1.25   --满配屏息
PUBG.m16a4aldx = 0.74   --满配蹲下
PUBG.m16a44x = 3.10     --空配4倍站
PUBG.m16a44xdx = 2.30   --空配4倍蹲
PUBG.m16a4al4x = 2.30   --满配4倍站
PUBG.m16a4al4xdx = 1.70 --满配4倍蹲

PUBG.m416 = 0.55       --空配站着
PUBG.m416bx = 0.70     --空配屏息
PUBG.m416dx = 0.45     --空配蹲下
PUBG.m416al = 1.00     --满配站着
PUBG.m416albx = 1.34   --满配屏息
PUBG.m416aldx = 0.87   --满配蹲下
PUBG.m4164x = 1.34     --空配4倍站
PUBG.m4164xdx = 1.05  	--空配4倍蹲
PUBG.m416al4x = 1.77   --满配4倍站
PUBG.m416al4xdx = 1.40 --满配4倍蹲

PUBG.aug = 1.93       --空配站着
PUBG.augbx = 2.45     --空配屏息
PUBG.augdx = 1.52     --空配蹲下
PUBG.augal = 1.54     --满配站着
PUBG.augalbx = 2.00   --满配屏息
PUBG.augaldx = 1.35   --满配蹲下
PUBG.aug4x = 2.20     --空配4倍站
PUBG.aug4xdx = 1.75   --空配4倍蹲
PUBG.augal4x = 1.79   --满配4倍站
PUBG.augal4xdx = 1.54 --满配4倍蹲

PUBG.g36c = 2.20       --空配站着
PUBG.g36cbx = 2.82     --空配屏息
PUBG.g36cdx = 1.82     --空配蹲下
PUBG.g36cal = 1.62     --满配站着
PUBG.g36calbx = 2.06   --满配屏息
PUBG.g36caldx = 1.34   --满配蹲下
PUBG.g36c4x = 5.00     --空配4倍站
PUBG.g36c4xdx = 3.80   --空配4倍蹲
PUBG.g36cal4x = 4.00   --满配4倍站
PUBG.g36cal4xdx = 3.44 --满配4倍蹲

PUBG.qbz95 = 1.48       --空配站着
PUBG.qbz95bx = 1.98     --空配屏息
PUBG.qbz95dx = 1.18     --空配蹲下
PUBG.qbz95al = 1.23     --满配站着
PUBG.qbz95albx = 1.65   --满配屏息
PUBG.qbz95aldx = 1.05   --满配蹲下
PUBG.qbz954x = 1.37     --空配4倍站
PUBG.qbz954xdx = 1.02   --空配4倍蹲
PUBG.qbz95al4x = 1.77   --满配4倍站
PUBG.qbz95al4xdx = 1.41 --满配4倍蹲

PUBG.scarl = 1.50       --空配站着
PUBG.scarlbx = 2.02     --空配屏息
PUBG.scarldx = 1.20     --空配蹲下
PUBG.scarlal = 1.48     --满配站着
PUBG.scarlalbx = 1.35   --满配屏息
PUBG.scarlaldx = 1.25   --满配蹲下
PUBG.scarl4x = 4.97     --空配4倍站
PUBG.scarl4xdx = 3.85   --空配4倍蹲
PUBG.scarlal4x = 4.01   --满配4倍站
PUBG.scarlal4xdx = 3.34 --满配4倍蹲

PUBG.ump45 = 0.96       --空配站着
PUBG.ump45bx = 1.25     --空配屏息
PUBG.ump45dx = 0.80     --空配蹲下
PUBG.ump45al = 0.74     --满配站着
PUBG.ump45albx = 0.95   --满配屏息
PUBG.ump45aldx = 0.68   --满配蹲下
PUBG.ump454x = 2.75     --空配4倍站
PUBG.ump454xdx = 2.15   --空配4倍蹲
PUBG.ump45al4x = 1.95   --满配4倍站
PUBG.ump45al4xdx = 1.57 --满配4倍蹲

PUBG.pp19 = 5.40       --空配站着
PUBG.pp19bx = 6.65     --空配屏息
PUBG.pp19dx = 4.00     --空配蹲下
PUBG.pp19al = 4.30     --满配站着
PUBG.pp19albx = 5.35   --满配屏息
PUBG.pp19aldx = 3.34   --满配蹲下
PUBG.pp194x = 13.3     --空配4倍站
PUBG.pp194xdx = 10.5   --空配4倍蹲
PUBG.pp19al4x = 10.2   --满配4倍站
PUBG.pp19al4xdx = 8.70 --满配4倍蹲

PUBG.vss = 0.55       --空配站着
PUBG.vssbx = 0.50     --空配屏息
PUBG.vssdx = 0.40     --空配蹲下
PUBG.vssal = 0.45     --满配站着
PUBG.vssalbx = 0.40   --满配屏息
PUBG.vssaldx = 0.30   --满配蹲下
PUBG.vss4x = 0.55     --空配4倍站
PUBG.vss4xdx = 0.38   --空配4倍蹲
PUBG.vssal4x = 0.45   --满配4倍站
PUBG.vssal4xdx = 0.33 --满配4倍蹲

PUBG.sks = 1.65       --空配站着
PUBG.sksbx = 2.35     --空配屏息
PUBG.sksdx = 1.10     --空配蹲下
PUBG.sksal = 1.03     --满配站着
PUBG.sksalbx = 1.45   --满配屏息
PUBG.sksaldx = 0.75   --满配蹲下
PUBG.sks4x = 4.20     --空配4倍站
PUBG.sks4xdx = 2.85   --空配4倍蹲
PUBG.sksal4x = 2.70   --满配4倍站
PUBG.sksal4xdx = 1.75 --满配4倍蹲

PUBG.mini = 1.30       --空配站着
PUBG.minibx = 1.75     --空配屏息
PUBG.minidx = 1.00     --空配蹲下
PUBG.minial = 1.55     --满配站着
PUBG.minialbx = 1.85   --满配屏息
PUBG.minialdx = 1.12   --满配蹲下
PUBG.mini4x = 3.35     --空配4倍站
PUBG.mini4xdx = 2.45   --空配4倍蹲
PUBG.minial4x = 3.85   --满配4倍站
PUBG.minial4xdx = 2.75 --满配4倍蹲
--------------------------------------------------------------------------
----------------           执行区压枪参数     ------------------------------
--------------------------------------------------------------------------
