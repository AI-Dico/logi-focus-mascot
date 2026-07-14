# logi focus mascot

> **logi focus** 마스코트 · 애니메이션 스프라이트 시안
> Animated sprite set of the logi focus plush mascot — 3 colorways × 4 states.

크림 실리콘 플러시 키링에서 출발한 **logi focus** 마스코트를, 게임/앱에 바로 쓸 수 있는
투명 배경 애니메이션 스프라이트로 만든 세트입니다. 세 가지 컬러(크림·블루·핑크)와
네 가지 동작 상태(idle · focus · walk · success)로 구성됩니다.

---

## Animations

| | idle | focus | walk | success |
|:--:|:--:|:--:|:--:|:--:|
| **Cream** | ![cream idle](./animations/cream-idle.gif) | ![cream focus](./animations/cream-focus.gif) | ![cream walk](./animations/cream-walk.gif) | ![cream success](./animations/cream-success.gif) |
| **Blue** | ![blue idle](./animations/blue-idle.gif) | ![blue focus](./animations/blue-focus.gif) | ![blue walk](./animations/blue-walk.gif) | ![blue success](./animations/blue-success.gif) |
| **Pink** | ![pink idle](./animations/pink-idle.gif) | ![pink focus](./animations/pink-focus.gif) | ![pink walk](./animations/pink-walk.gif) | ![pink success](./animations/pink-success.gif) |

- **idle** — 잔잔한 숨쉬기 + 중간에 활짝 웃는 표정
- **focus** — 눈을 지그시 감고 집중 모드에 들어가는 상태
- **walk** — 발을 교대로 내딛는 걷기 루프
- **success** — 양팔 만세 + 스쿼시-스트레치 축하 바운스

## Sprite sheets

`spritesheets/<color>/` 에 실사용 에셋이 들어 있습니다.

```
spritesheets/<color>/
├── sprite-sheet-alpha.png   # 투명 배경 아톰라스
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
