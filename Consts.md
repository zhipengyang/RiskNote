####1. apply_risk
    
    const APPLY_RISK_TYPE_LOAN_FIRST = 1; //单期贷首次
    const APPLY_RISK_TYPE_LOAN_MULTIPLE = 2; //单期贷多次
    const APPLY_RISK_TYPE_BLIND_GRANT = 3; //盲放
    const APPLY_RISK_TYPE_MULTIPLE_LOAN = 4; //多期贷
    const APPLY_RISK_TYPE_BACK_USER = 5; //回流客
    
    self::APPLY_RISK_PERIOD_6 => '6期',
    self::APPLY_RISK_PERIOD_3 => '3期',
    self::APPLY_RISK_PERIOD_MANY => '历史多期贷',
    self::APPLY_RISK_PERIOD_ONE => '单期贷',
    
    const APPLY_RISK_STATUS_INITIAL = 1; //初始状态
    const APPLY_RISK_STATUS_ONE_START = 2; //一审开始
    const APPLY_RISK_STATUS_ONE_END = 3; //一审结束
    const APPLY_RISK_STATUS_TWO_START = 4; //二审开始
    const APPLY_RISK_STATUS_TWO_END = 5; //二审结束
    
    const APPLY_RISK_RESULT_PASS = 'pass'; //通过
    const APPLY_RISK_RESULT_REFUSE = 'refuse'; //拒绝
    const APPLY_RISK_RESULT_MANUAL = 'manual'; //人工审核
    const APPLY_RISK_RESULT_EXCEPTION = 'exception'; //审核中

####2. 第三方数据类型

    const BR_DATA   = 'br_fraud';
    const TX_ED     = 'tx_ed';
    const QH_CREDOO = 'qh_credoo';
    const QH_RSKDOO = 'qh_rskdoo';
    const QH_LOANEE = 'qh_loanee';
    const UNIONPAY  = 'unionpay';
    const TONGDUN   = 'tongdun';
    const JXL       = 'juxinli_phone_collect';
    const ZHIMA_SCORE = 'zhima_score';
    const ZHIMA_BLACK = 'zhima_black';
    const ZHIMA_ANTI_FRAUD_SCORE = 'zhima_anti_fraud_score';    //芝麻反欺诈信用积分
    const ZHIMA_ANTI_FRAUD_VERIFY = 'zhima_anti_fraud_verify';  //芝麻欺诈信息验证
    const ZHIMA_IVS   = 'zhima_ivs';
    const ANTI_FRAUD_TWO_POINT_ZERO =  'anti_fraud_version_two_point_zero';
    const ANTI_FRAUD  = 'anti_fraud';
    const ANTI_FRAUD_OLD  = 'anti_fraud_old';
    const BAIQISHI    = 'baiqishi';
    const BQS_DATA    = 'bqs_data';
    const BQS_HIT     = 'bqs_hit_rules';
    const SUANHUA     = 'suanhua';
    const YD_FRAUD    = 'yd_fraud';
    const YD_DISH     = 'yd_dish';             //法院失信个人
    const YD_P2P      = 'yd_p2p';              //失信名单
    const YD_TERROR   = 'yd_terror';
    const YD_ECON     = 'yd_econ';
    const YD_LEAK     = 'yd_leak';             //身份证泄漏查询
    const YD_ACCURATE = 'yd_accurate';
    const YD_BORROW   = 'yd_borrow';           //信用魔镜借款信息查询
    const YD_BANKCARD = 'yd_bankcard';
    const YD_DISHONESTY = 'yd_dishonesty';
    const UNICOM_VERIFY = 'unicom_verify'; //联通的验证信息
    const UNICOM_STATE     = 'unicom_state'; //联通的在网状态
    const UNICOM_LENGTH    = 'unicom_length'; //联通的在网时长
    const BIZ_REPAY = 'biz_repay'; //biz的还款计划
    const BD_CONTENT = 'bd_content';
    const BD_CONTENT_NEW = 'bd_content_new';
    const JD_CREDIT        = 'jd_credit';     //京东白条信用分
    const JD_ADDRESS_BLACK = 'jd_address_black'; //地址是否涉黑
    const JD_BLACK_LIST    = 'jd_black_list';    //黑名单
    const JD_XB_CREDIT     = 'jd_xb_credit';     //京东小白信用分
    const JD_PERSONA       = 'jd_persona';       //网购画像
    const JD_SS_SCORE       = 'jd_ss_score';
    const JJD_CREDIT       = 'jjd_credit';      //金节点消费数据
    const JJD_OVERDUE      = 'jjd_overdue';     //金节点逾期数据
    const BAIQISHI_ZIXINYUN= 'baiqishi_zixinyun'; //白骑士资信云
    const NSFS             = 'nsfs';            //上海资信
    const ZHIMA_ANTI_FRAUD = 'zhima_antifraud'; //芝麻欺诈关注清单
    const ZHIMA_DAS        = 'zhima_das'; //芝麻元素表
    const YD_SECURITY      = 'youdun_security'; //有盾社保
    const YD_FUND          = 'youdun_fund'; //有盾公积金
    const HAITUN           = 'haitun'; //海通信用
    const YD_ALIPAY        = 'youdun_alipay'; //有盾公支付宝
    const YD_JINGDONG      = 'youdun_jingdong';//有盾京东
    const YD_TAOBAO      = 'youdun_taobao';//有盾京东
    const YD_INSURANCE_CAR      = 'youdun_insurance_car';//有盾车险
    const YD_QQ            = 'youdun_qq'; //有盾QQ
    const IPIP_GEO = 'ipip_geo'; //ipip.net提供的IP信息
    const BD_FINANCE_MALL = 'bd_finance_mall'; //百度金融商城运营商信息
    const SHANGSHU_YYS = 'shangshu_yys'; //ipip.net提供的IP信息
    const JXL_INSURANCE = 'jxl_insurance';//聚信力寿险
    const PY_CAR       = 'py_car';//鹏元车辆相关数据 
    const PY_CARPRICE  = 'py_carprice';//鹏元车辆估价信息 
    const PY_CARPROD   = 'py_carprod';//鹏元车产信息
    const PY_CAR_BASEINFO = 'py_car_baseinfo'; //鹏元车辆相关数据 -基本信息
    const PY_CAR_CARSTATUS = 'py_car_carstatus'; //鹏元车辆相关数据 -机动车状态
    const PY_CAR_REGISTER = 'py_car_register'; //鹏元车辆相关数据 -初次登记是日期一致性
    const PY_CARPROD_HASCAR = 'py_carprod_hascar'; //鹏元车产信息-是否有车
    const PY_CARPROD_CARASSET = 'py_carprod_carasset'; //鹏元车产信息-个人车产价值情况
    const YD_ZHENGXIN        = 'youdun_zhengxin'; //有盾人行征信
    const SLOPS_EMAIL_BILL = 'email_bill'; //数立邮箱账单
    const BD_CREDIT = 'baidu_credit'; //百度信用
    const PY_VEHICLE = 'pengyuan_vehicle';
    const BAIQISHI_CREDIT = 'baiqishi_credit';//白骑士信贷报告
    const XCLOUD_SCORE    = 'xcloud_score'; //氪信分
    const XCLOUD_FRAUD    = 'xcloud_fraud'; //氪信反欺诈
    const BD_PS_PREA = 'baidu_panshi_prea';//百度磐石系统PREA信用分数
    const BD_PS_LBS = 'baidu_panshi_lbs';//百度磐石系统LBS地址校验
    const BD_PS_DUOTOU = 'baidu_panshi_duotou';//百度磐石系统多头信息查询
    const BD_PS_BLACK = 'baidu_panshi_black';//百度磐石系统黑产信息查询
    const TX_LIVING_BODY = 'tx_living_body'; //腾讯活体
    const XY_BLACK = 'xinyan_black'; // 新颜 负面拉黑
    const XY_WHITE = 'xinyan_white'; // 新颜 负面洗白
    const SHUMEI_MULTILOAN = 'shumei_multiloan';
    const SHUMEI_YELLOW_PAGE = 'shumei_yellow_page';
    const SHUMEI_CREDIBLE_LEVEL = 'shumei_credible_level';
    const SHUMEI_MOBILE_LABEL = 'shumei_mobile_label';
    const SHUMEI_CREDIT_ANALYSE = 'shumei_credit_analyse';
    const SHUMEI_MALAGENT = 'shumei_malagent';
    const SHUMEI_OVERDUE = 'shumei_overdue';
    const XY_MODEL = 'xinyan_model'; // 新颜 模型
    const BR_CHECK_APPLY = 'bairong_check_apply'; // 百融多次申请查询
    const BR_SPECIAL_LIST = 'bairong_special_list'; // 百融多次申请查询
    const XY_OLD_MODEL = 'xinyan_old_model';
    const FBI_SCORE = 'FBIScore'; //腾讯欺诈行为调查
    
####3. Process State

    self::PROCESS_STATE_START => '审核开始',
    self::PROCESS_STATE_ZHIMA => '芝麻分',
    self::PROCESS_STATE_BASE => '基础审核',
    self::PROCESS_STATE_BIZ => 'biz',
    self::PROCESS_STATE_ANTI => '腾讯天御',
    self::PROCESS_STATE_ZM_BLACK => '芝麻黑名单',
    self::PROCESS_STATE_BD => '百度',
    self::PROCESS_STATE_BQS => '白骑士',
    self::PROCESS_STATE_TD => '同盾',
    self::PROCESS_STATE_JD => '京东',
    self::PROCESS_STATE_FUND => '公积金',
    self::PROCESS_STATE_JD_PERSONA => '京东网购画像',
    self::PROCESS_STATE_HT => '海豚',
    self::PROCESS_STATE_JXL => '聚信立',
    self::PROCESS_STATE_SH => '算话',
    self::PROCESS_STATE_PASS => '审核通过',
    self::PROCESS_STATE_REFUSE => '审核拒绝',
    self::PROCESS_STATE_ONE_START => '一审开始',
    self::PROCESS_STATE_ONE_PASS => '一审通过',
    self::PROCESS_STATE_ONE_REFUSE => '一审拒绝',
    self::PROCESS_STATE_TWO_START => '二审开始',
    self::PROCESS_STATE_TWO_PASS => '二审通过',
    self::PROCESS_STATE_TWO_REFUSE => '二审拒绝',
    self::PROCESS_LIVING_BODY_STATE_NOTIFY => '通知业务方',
    self::PROCESS_AUDIT_STATE_PASS => '人工审核通过',
    self::PROCESS_AUDIT_STATE_REFUSE => '人工审核拒绝',
    self::PROCESS_STATE_PASSED => '通过',
    self::PROCESS_STATE_REFUSED => '拒绝',
    self::PROCESS_STATE_COMPLETE => '审核完成',
    self::PROCESS_STATE_NOTIFY_BUSINESS => '通知业务方',
    self::PROCESS_STATE_MODEL_DECISION => '模型决策',
    self::PROCESS_STATE_DECISION => '决策',
    self::PROCESS_STATE_MODEL_DECISION =>'模型决策 ',
    self::PROCESS_STATE_RULE_REFUSE =>'规则拒绝',
    self::PROCESS_STATE_COMPLETE_REFUSE =>'审核完成拒绝',
    self::PROCESS_STATE_COMPLETE_PASS =>'审核完成通过',
    self::PROCESS_STATE_MAKE_MANUAL =>'创建人工审核订单',

####4. 大数据模型

    const BIG_DATA_MODEL_TYPE_ZK = 1; //中科模型
    const BIG_DATA_MODEL_TYPE_LH = 2; //刘航模型
    const BIG_DATA_MODEL_TYPE_RONG_360 = 3; //融360模型
    const BIG_DATA_MODEL_TYPE_NAVIGATE_360 = 4; //导航360
    const BIG_DATA_MODEL_TYPE_CASH_WHITE_CARD = 5; //现金白卡
    const BIG_DATA_MODEL_TYPE_XT_JM = 7;
    
    public static $bigDataModels = [
        'A66O6T3DXGB_ZK_20171013' => self::BIG_DATA_MODEL_TYPE_ZK, //中科五级模型，与大数据约定好传1
        'A66O3T3DGBD_BAG_ZK_20171020' => self::BIG_DATA_MODEL_TYPE_ZK, //中科五级模型2，与大数据约定好传1
        'A50O15T1DADA_LH_20171018' => self::BIG_DATA_MODEL_TYPE_LH, //刘航模型，与大数据约定好传2
        'A60O13T3DXGB_FD_20171120' => self::BIG_DATA_MODEL_TYPE_RONG_360, //融360模型
        'A50O13T3DXGB_FD_20171204' => self::BIG_DATA_MODEL_TYPE_CASH_WHITE_CARD, //现金白卡模型
        'A30O8T3DXGB_FD_20171205'  => self::BIG_DATA_MODEL_TYPE_NAVIGATE_360, //导航360模型
        'A60O6T3DXGB_ZK_20171123' => self::BIG_DATA_MODEL_TYPE_ZK, //范迪中科模型
        'A60O13T3DXGB_FD_20171124' => self::BIG_DATA_MODEL_TYPE_ZK, //范迪中科模型
        'A10O10T1DXGB_XT_20171223' => self::BIG_DATA_MODEL_TYPE_XT_JM, //徐婷静默模型
    ];

####5. 算法查询

    public static $monitorType = [
        self::TONGDUN   => 'common\modules\risk\models\TdMonitor'
    ];

    //策略选择算法
    public static $strategySelectionType = [
        self::STRATEGY_SELECTION_TYPE_DEFAULT => 'common\modules\risk\strategySelect\DefaultSelection',
    ];

    //反欺诈选择算法
    public static $fraudSelectionType = [
        self::FRAUD_SELECTION_TYPE_DEFAULT => 'common\modules\risk\fraudSelect\DefaultFraudSelection',
        self::FRAUD_SELECTION_TYPE_MERGE => 'common\modules\risk\fraudSelect\MergeFraudSelection',
    ];

    //决策算法
    public static $decisionType = [
        self::DECISION_TYPE_NO => 'common\modules\risk\decision\NoDecision',
        self::DECISION_TYPE_MULTI => 'common\modules\risk\decision\MultiDecision',
    ];

    //授信对应的类型
    public static $creditSelectionType = [
        self::YD_FUND => 'common\modules\risk\credit\FundCredit',
        self::HAITUN => 'common\modules\risk\credit\HaitunCredit'
    ];

    //规则组对应算法
    public static $ruleGroupSelectionType = [
        self::RULE_GROUP_SELECTION_TYPE_DEFAULT => 'common\modules\risk\ruleGroupSelect\DefaultRuleGroupSelection',
    ];
