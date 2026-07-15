# logi focus mascot

> **logi focus** 마스코트 · 애니메이션 스프라이트 세트
> Animated sprite set of the logi focus plush mascot — **3 colorways × 21 states** (4 base + 17 emotions).

크림 실리콘 플러시 키링에서 출발한 **logi focus** 마스코트를, 게임/앱에 바로 쓸 수 있는
투명 배경 애니메이션 스프라이트로 만든 세트입니다. 세 가지 컬러(크림·블루·핑크)와
기본 4상태 + 17가지 감정 표현으로 구성됩니다. 눈·입은 최소한으로 두고 자세·타이밍으로 감정을 표현합니다.

---

## 기본 상태 · Base states

| 상태 | Cream | Blue | Pink |
|:--|:--:|:--:|:--:|
| **중립/대기** `idle` | ![](./animations/cream-idle.gif) | ![](./animations/blue-idle.gif) | ![](./animations/pink-idle.gif) |
| **집중** `focus` | ![](./animations/cream-focus.gif) | ![](./animations/blue-focus.gif) | ![](./animations/pink-focus.gif) |
| **걷기** `walk` | ![](./animations/cream-walk.gif) | ![](./animations/blue-walk.gif) | ![](./animations/pink-walk.gif) |
| **성취** `success` | ![](./animations/cream-success.gif) | ![](./animations/blue-success.gif) | ![](./animations/pink-success.gif) |

- **idle** 잔잔한 숨쉬기 + 웃음 · **focus** 눈 감고 집중 · **walk** 걷기 루프 · **success** 만세 축하

## 코어 감정 · Core emotions

| 상태 | Cream | Blue | Pink |
|:--|:--:|:--:|:--:|
| **기쁨** `joy` | ![](./animations/cream-joy.gif) | ![](./animations/blue-joy.gif) | ![](./animations/pink-joy.gif) |
| **슬픔** `sad` | ![](./animations/cream-sad.gif) | ![](./animations/blue-sad.gif) | ![](./animations/pink-sad.gif) |
| **놀람** `surprise` | ![](./animations/cream-surprise.gif) | ![](./animations/blue-surprise.gif) | ![](./animations/pink-surprise.gif) |
| **격려** `encouraging` | ![](./animations/cream-encouraging.gif) | ![](./animations/blue-encouraging.gif) | ![](./animations/pink-encouraging.gif) |
| **경고** `alert` | ![](./animations/cream-alert.gif) | ![](./animations/blue-alert.gif) | ![](./animations/pink-alert.gif) |

## 확장 감정 · Extended emotions

| 상태 | Cream | Blue | Pink |
|:--|:--:|:--:|:--:|
| **평온** `relaxed` | ![](./animations/cream-relaxed.gif) | ![](./animations/blue-relaxed.gif) | ![](./animations/pink-relaxed.gif) |
| **기대** `anticipation` | ![](./animations/cream-anticipation.gif) | ![](./animations/blue-anticipation.gif) | ![](./animations/pink-anticipation.gif) |
| **걱정** `anxious` | ![](./animations/cream-anxious.gif) | ![](./animations/blue-anxious.gif) | ![](./animations/pink-anxious.gif) |
| **분노** `angry` | ![](./animations/cream-angry.gif) | ![](./animations/blue-angry.gif) | ![](./animations/pink-angry.gif) |
| **졸림** `sleepy` | ![](./animations/cream-sleepy.gif) | ![](./animations/blue-sleepy.gif) | ![](./animations/pink-sleepy.gif) |
| **지루함** `bored` | ![](./animations/cream-bored.gif) | ![](./animations/blue-bored.gif) | ![](./animations/pink-bored.gif) |
| **사랑** `love` | ![](./animations/cream-love.gif) | ![](./animations/blue-love.gif) | ![](./animations/pink-love.gif) |
| **결심** `determined` | ![](./animations/cream-determined.gif) | ![](./animations/blue-determined.gif) | ![](./animations/pink-determined.gif) |

## 보조 감정 · More expressions

| 상태 | Cream | Blue | Pink |
|:--|:--:|:--:|:--:|
| **의심** `thinking` | ![](./animations/cream-thinking.gif) | ![](./animations/blue-thinking.gif) | ![](./animations/pink-thinking.gif) |
| **혐오** `disgust` | ![](./animations/cream-disgust.gif) | ![](./animations/blue-disgust.gif) | ![](./animations/pink-disgust.gif) |
| **부끄러움** `shy` | ![](./animations/cream-shy.gif) | ![](./animations/blue-shy.gif) | ![](./animations/pink-shy.gif) |
| **산만** `distracted` | ![](./animations/cream-distracted.gif) | ![](./animations/blue-distracted.gif) | ![](./animations/pink-distracted.gif) |

---

## 롱 idle · Long idle loops

세그먼트 분할 생성(숨쉬기·웃음·깜빡, 각 8프레임 · 중립 포즈로 시작/종료) 후 이어붙인 긴 idle 루프입니다.
Long idle loops stitched from separately generated segments (breath · smile · blink), each anchored to the same neutral pose.

| 버전 | Cream | Blue | Pink |
|:--|:--:|:--:|:--:|
| **D** raw 스티치 · 4초 (실제 24프레임) | ![](./animations/long/cream-idle-D-raw.gif) | ![](./animations/long/blue-idle-D-raw.gif) | ![](./animations/long/pink-idle-D-raw.gif) |
| **E** 세그+모션보간 · 8초 | ![](./animations/long/cream-idle-E-8s.gif) | ![](./animations/long/blue-idle-E-8s.gif) | ![](./animations/long/pink-idle-E-8s.gif) |
| **F** 시퀀스 연출 · 9.5초 (숨쉬다 가끔 웃고 깜빡) | ![](./animations/long/cream-idle-F-10s.gif) | ![](./animations/long/blue-idle-F-10s.gif) | ![](./animations/long/pink-idle-F-10s.gif) |

---

## Sprite sheets

`spritesheets/<color>/` 에 실사용 에셋이 들어 있습니다.

```
spritesheets/<color>/
├── sprite-sheet-alpha.png   # 투명 배경 아톰라스 (21상태)
├── manifest.json            # 런타임 좌표 (frame_layout · fps · loop)
└── frames/<state>/*.png     # 상태별 개별 프레임
```

런타임 코드는 `manifest.json` 의 `frame_layout` 사각형만 샘플링하면 됩니다.

---

## License

© 2026 Dcode Labs. All rights reserved.

"logi focus" 및 logi focus 마스코트 캐릭터와 이 저장소의 모든 아트워크·애니메이션·스프라이트
에셋은 Dcode Labs 의 자산입니다. 본 에셋은 **쇼케이스·참고 목적으로만** 공개되며,
사전 서면 허가 없이 사용·복제·수정·배포·2차적저작물 제작을 허가하지 않습니다.

These assets are published for showcase and reference only. No license is granted to use,
reproduce, modify, or distribute them without prior written permission.

문의 · Inquiries: **support@1pass.dev**
