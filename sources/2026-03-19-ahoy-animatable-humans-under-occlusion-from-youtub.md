# AHOY! Animatable Humans under Occlusion from YouTube Videos with Gaussian Splatting and Video Diffusion Priors

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-03-19
**링크**: http://arxiv.org/abs/2603.17975v1

## 💡 핵심 인사이트

비디오 디퓨전 모델을 3D 가우시안 스플래팅의 사전 지식으로 활용하여, 가림이 심한 야생 단안 영상에서도 완전한 애니메이션 가능 3D 인간 아바타 복원이 가능함을 보였다.

## 📖 분석

## AHOY: 가려진 유튜브 영상에서 애니메이션 가능한 3D 인간 복원

AHOY는 단안(monocular) 야생 영상에서 심한 가림(occlusion)이 존재하더라도 완전한 애니메이션 가능 3D 가우시안 아바타를 복원하는 방법을 제시한다. 기존 방법들은 가림이 없는 입력, 즉 완전히 보이는 피사체를 전제로 하여 실제 환경의 대부분의 영상을 처리할 수 없었다. 가구, 물체, 다른 사람에 의해 일상적으로 가려지는 현실 영상에서의 복원은 근본적 난제를 수반한다: 신체의 넓은 영역이 관측되지 않을 수 있고, 포즈별 다시점 감독이 부족하다.

AHOY의 핵심 기여는 **3D Gaussian Splatting**과 **비디오 디퓨전 프라이어(Video Diffusion Priors)**를 결합한 접근법이다. Gaussian Splatting은 최근 3D 장면 표현에서 NeRF의 대안으로 부상한 기법으로, 명시적 가우시안 원시체를 활용해 실시간 렌더링과 높은 품질을 동시에 달성한다. 비디오 디퓨전 모델은 관측되지 않은 신체 영역을 생성적으로 보완하는 강력한 사전 지식(prior)으로 활용된다.

이 연구는 컴퓨터 비전과 생성 모델의 교차점에 위치하며, 디퓨전 모델의 활용 범위가 이미지 생성을 넘어 3D 복원 문제의 정규화(regularization)로 확장되고 있음을 보여준다. 특히 YouTube 같은 비정제 영상에서 직접 아바타를 구축할 수 있다는 점에서, 대규모 스튜디오 설비 없이도 디지털 휴먼 생성이 가능해지는 민주화 방향을 제시한다.

## 📐 개념

- [[concepts/gaussian-splatting.md|gaussian-splatting]]
- [[concepts/video-diffusion.md|video-diffusion]]
- [[concepts/3d-human-reconstruction.md|3d-human-reconstruction]]

---
_LLM 분석으로 재생성됨_

---
**관련**: [[concepts/latent-diffusion.md|latent diffusion]]
