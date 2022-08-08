## TUICallKit (含 UI 接口)

TUICallKit API 是音视频通话组件的**含 UI 接口**，使用TUICallKit API，您可以通过简单接口快速实现一个类微信的音视频通话场景。

| API | 描述 |
|-----|-----|
| [createInstance](https://tcloud-doc.isd.com/document/product/647/78750?!preview#createinstance) | 创建 TUICallKit 实例（单例模式） |
| [setSelfInfo](https://tcloud-doc.isd.com/document/product/647/78750?!preview#setselfinfo) | 设置用户的头像、昵称             |
| [call](https://tcloud-doc.isd.com/document/product/647/78750?!preview#call) | 发起 1v1 通话                    |
| [groupCall](https://tcloud-doc.isd.com/document/product/647/78750?!preview#groupcall) | 发起群组通话                     |
| [joinInGroupCall](https://tcloud-doc.isd.com/document/product/647/78750?!preview#joiningroupcall) | 主动加入当前的群组通话中         |
| [setCallingBell](https://tcloud-doc.isd.com/document/product/647/78750?!preview#setcallingbell) | 设置自定义来电铃音               |
| [enableMuteMode](https://tcloud-doc.isd.com/document/product/647/78750?!preview#enablemutemode) | 开启/关闭静音模式                |
| [enableFloatWindow](https://tcloud-doc.isd.com/document/product/647/78750?!preview#enablefloatwindow) | 开启/关闭悬浮窗功能              |


## TUICallEngine (无 UI 接口)

TUICallEngine API 是音视频通话组件的**无 UI 接口**，如果 TUICallKit 的交互并不满足您的需求，您可以使用这套 API 根据您的业务需求自定义封装。

| API | 描述 |
|-----|-----|
| [createInstance](https://tcloud-doc.isd.com/document/product/647/78749?!preview#createinstance) | 创建 TUICallEngine 实例（单例模式）                         |
| [destroyInstance](https://tcloud-doc.isd.com/document/product/647/78749?!preview#destroyinstance) | 销毁 TUICallEngine 实例（单例模式）                         |
| [init](https://tcloud-doc.isd.com/document/product/647/78749?!preview#init) | 完成音视频通话基础能力的鉴权                                |
| [addObserver](https://tcloud-doc.isd.com/document/product/647/78749?!preview#addobserver) | 增加事件回调                                                |
| [removeObserver](https://tcloud-doc.isd.com/document/product/647/78749?!preview#removeobserver) | 移除回调接口                                                |
| [call](https://tcloud-doc.isd.com/document/product/647/78749?!preview#call) | 发起 1v1 通话                                               |
| [groupCall](https://tcloud-doc.isd.com/document/product/647/78749?!preview#groupcall) | 发起群组通话                                                |
| [accept](https://tcloud-doc.isd.com/document/product/647/78749?!preview#accept) | 接听通话                                                    |
| [reject](https://tcloud-doc.isd.com/document/product/647/78749?!preview#reject) | 拒绝通话                                                    |
| [hangup](https://tcloud-doc.isd.com/document/product/647/78749?!preview#hangup) | 结束通话                                                    |
| [ignore](https://tcloud-doc.isd.com/document/product/647/78749?!preview#ignore) | 忽略通话                                                    |
| [inviteUser](https://tcloud-doc.isd.com/document/product/647/78749?!preview#inviteuser) | 在群组通话中，邀请其他人加入                                |
| [joinInGroupCall](https://tcloud-doc.isd.com/document/product/647/78749?!preview#joiningroupcall) | 主动加入当前的群组通话中                                    |
| [switchCallMediaType](https://tcloud-doc.isd.com/document/product/647/78749?!preview#switchcallmediatype) | 切换通话媒体类型，比如视频通话切音频通话                    |
| [startRemoteView](https://tcloud-doc.isd.com/document/product/647/78749?!preview#startremoteview) | 开始订阅远端用户视频流                                      |
| [stopRemoteView](https://tcloud-doc.isd.com/document/product/647/78749?!preview#stopremoteview) | 停止订阅远端用户视频流                                      |
| [openCamera](https://tcloud-doc.isd.com/document/product/647/78749?!preview#opencamera) | 开启摄像头                                                  |
| [closeCamara](https://tcloud-doc.isd.com/document/product/647/78749?!preview#closecamara) | 关闭摄像头                                                  |
| [switchCamera](https://tcloud-doc.isd.com/document/product/647/78749?!preview#switchcamera) | 切换前后摄像头                                              |
| [openMicrophone](https://tcloud-doc.isd.com/document/product/647/78749?!preview#openmicrophone) | 打开麦克风                                                  |
| [closeMicrophone](https://tcloud-doc.isd.com/document/product/647/78749?!preview#closemicrophone) | 关闭麦克风                                                  |
| [selectAudioPlaybackDevice](https://tcloud-doc.isd.com/document/product/647/78749?!preview#selectaudioplaybackdevice) | 选择音频播放设备（听筒/扬声器）                             |
| [setSelfInfo](https://tcloud-doc.isd.com/document/product/647/78749?!preview#setselfinfo) | 设置用户的昵称、头像                                        |
| [enableMultiDeviceAbility](https://tcloud-doc.isd.com/document/product/647/78749?!preview#enablemultideviceability) | 开启/关闭 TUICallEngine 的多设备登录模式 （尊享版套餐支持） |

## TUICallObserver 
TUICallObserver 是 TUICallEngine 对应的回调事件类，您可以通过此回调，来监听自己感兴趣的回调事件。

| API | 描述 |
|-----|-----|
| [onError](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onerror) | 通话过程中错误回调           |
| [onCallReceived](https://tcloud-doc.isd.com/document/product/647/78751?!preview#oncallreceived) | 通话请求的回调               |
| [onCallCancelled](https://tcloud-doc.isd.com/document/product/647/78751?!preview#oncallcancelled) | 通话取消的回调               |
| [onCallBegin](https://tcloud-doc.isd.com/document/product/647/78751?!preview#oncallbegin) | 通话接通的回调               |
| [onCallEnd](https://tcloud-doc.isd.com/document/product/647/78751?!preview#oncallend) | 通话结束的回调               |
| [onCallMediaTypeChanged](https://tcloud-doc.isd.com/document/product/647/78751?!preview#oncallmediatypechanged) | 通话的媒体类型发生改变的回调 |
| [onUserReject](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuserreject) | xxxx 用户拒绝通话的回调      |
| [onUserNoResponse](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onusernoresponse) | xxxx 用户不响应的回调        |
| [onUserLineBusy](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuserlinebusy) | xxxx 用户忙线的回调          |
| [onUserJoin](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuserjoin) | xxxx 用户加入通话的回调      |
| [onUserLeave](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuserleave) | xxxx 用户离开通话的回调      |
| [onUserVideoAvailable](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuservideoavailable) | xxx 用户是否有视频流的回调   |
| [onUserAudioAvailable](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuseraudioavailable) | xxx 用户是否有音频流的回调   |
| [onUserVoiceVolumeChanged](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onuservoicevolumechanged) | 所有用户音量大小的反馈回调   |
| [onUserNetworkQualityChanged](https://tcloud-doc.isd.com/document/product/647/78751?!preview#onusernetworkqualitychanged) | 所有用户网络质量的反馈回调   |


## 关键类型定义
| API | 描述 |
|-----|-----|
| TUICallDefine.MediaType | 通话的媒体类型，枚举类型：视频通话、语音通话 |
| TUICallDefine.Role | 通话的角色，枚举类型：主叫、被叫 |
| TUICallDefine.Status | 通话的状态，枚举类型：空闲、待接听、接听中 |
| TUICommonDefine.RoomId | 音视频房间Id，支持数字、字符串两种类型 |
| TUICommonDefine.Camera | 摄像头Id参数，枚举类型：前摄、后摄|
| TUICommonDefine.AudioPlaybackDevice | 声音的播放设备，枚举类型：扬声器、听筒 |
| TUICommonDefine.NetworkQualityInfo | 当前的网络质量信息 |







