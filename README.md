hostname = novel.test.onedayapp.cn

^https:\/\/novel\.test\.onedayapp\.cn\/login\/sync url script-response-body oneDayRead.js


var obj = JSON.parse($response.body);
obj.data.vip = 3;
obj.data.rewardEndTime = 3676971270888;
$done({body: JSON.stringify(obj)});
