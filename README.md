
# PyTorch KR Tutorial Competition 2018


## 개요


날이 갈수록 머신러닝 논문이 홍수처럼 쏟아지고 있습니다. 올해는 NIPS 에만 4900편 이상의 논문이 제출되었고, 그 외에도 ICML, ICLR, CVPR 등 다양한 학회와 Arxiv 에 끊임없이 새로운 논문이 공개되고 있습니다. 머신러닝 연구자와 개발자는 논문을 선별하고, 읽고 이해하고, 논문의 알고리즘을 실제로 검증해보는 데 이전보다 더욱 많은 시간을 들이게 되었습니다.

논문을 읽는 것은 쉬운 일이 아닙니다. 학회의 분량 및 형식 제한을 지키면서도 이론과 실험 결과를 모두 싣는 것이 어렵기 때문에, 많은 논문은 전문용어로 점철되고, 자세한 설명은 참고문헌을 언급함으로써 대신합니다. 이렇게 해당 분야의 초심자들에게 불친절한 논문일수록, 한 논문을 이해하기 위해서 여러 논문을 찾아보아야 합니다.

논문의 핵심 내용을 이해한 후에는 이를 명확히 이해하기 위해서 알고리즘을 구현해 보며 이해한 내용과 세부 동작이 일치하는지 확인해보아야 합니다. 또한 논문에서 제시하는 내용이 자신이 보유한 실제 데이터에도 적용이 되는지도 검증해야 합니다. 하지만 많은 논문에서 실험에 사용된 코드를 공개하지 않고, 그나마 공개된 코드들도 대부분은 소위 '실험용' 코드인 경우라 이해하기 힘든 경우가 많습니다.

그런데, 사실 새로운 논문을 이해하기 위해서 모든 사람이 꼭 여러 참고문헌을 찾아보고 코드를 밑바닥부터 구현하며 고생할 필요는 없습니다. 논문을 잘 이해한 사람들은 논문의 문장보다 핵심 개념을 훨씬 간단하게 풀어 설명할 수 있고, 이러한 설명을 들은 사람은 훨씬 빠르게 논문을 읽어내려갈 수 있습니다. 또한 저자가 공개한 공식 코드보다 논문을 잘 이해한 다른 사람의 구현이 더욱 간결하고 널리 쓰이는 경우도 상당히 많습니다.

다행히도, 머신러닝 분야에서는 자기가 읽은 논문들을 쉽게 풀어내어 블로그 등의 형태로 **튜토리얼** 을 만들고 공유하는 문화가 점점 퍼지고 있습니다. 하지만 한 가지 아쉬운 것은, 대부분의 튜토리얼이 영어로 제작되어있기 때문에, 영어에 친숙하지 않다면 접근하기 힘들거나 읽는 데도 많은 시간이 든다는 점입니다.

그래서 [**PyTorch KR**](https://www.facebook.com/groups/PyTorchKR/) 는 수많은 논문들을 빠르고 명확하게, 그리고 함께 이해하기 위해서 **Tutorial Competition 2018** 을 개최합니다. 특정 논문 또는 주제 (복수 논문) 를 선정하고, 자유 형식으로 한국어 튜토리얼을 만들어주세요!

수상자분들께는 상품과 함께 2019년 1월에 열릴 **PyTorch KR DevCon** 에서 자신이 만든 튜토리얼을 직접 소개할 기회를 드립니다!

## 규칙

* 개인 / 단체 참가 가능
* 분야 제한 없음 (ex. Vision, Language)
* 한국어 작성
    * 모든 용어를 한국어로 번역할 필요는 없음 (ex. Convolution, Attention, Dropout 등)
* 코드
    * 모든 코드는 Pseudocode 가 아닌, 실행 가능한 코드여야 함
    * [PyTorch 1.0](https://github.com/pytorch/pytorch/releases/tag/v1.0.0) 기반으로 작성
    * 출처를 밝히고 외부 코드 일부 사용 가능
    * 튜토리얼에 사용된 모든 데이터 및 dependency가 설치된 public docker image 작성
        * `docker run -it 도커 이미지 python main.py` 으로 결과 재현이 가능해야 함
        * Docker 에 익숙하지 않으신 분들은 [PyTorch Docker Tutorial](https://github.com/AppleHolic/PytorchDockerExample) 을 참고해주세요!
            * IlJi Choi (KakaoBrain) 님이 작성해 주셨습니다.

## 심사 기준
* 논문을 찾아보지 않아도 충분히 이해할 수 있는가
* 이미 좋은 기존 튜토리얼이 존재하지는 않는가
* 코드가 간결한가
* 코드가 모델, 이론에 대한 설명과 부합하는가
* 코드로 논문에서 보고하는 수준의 결과 재현이 가능한가


## 예시
- [Annotated Transformer (Harvard NLP)](http://nlp.seas.harvard.edu/2018/04/03/attention.html)
- [Differentiable Image Parameterizations (Mordvintsev et al.)](https://distill.pub/2018/differentiable-parameterizations/) 
- [Translation with a Sequence to Sequence Network and Attention (Sean Robertson)](https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html)
- [Variational AutoEncoder (이기창)](https://ratsgo.github.io/generative%20model/2018/01/27/VAE/)

## 제출 방법

본 행사 참가는 [GitHub 페이지](https://github.com/PyTorchKR/Tutorial-Competition-2018) 에 Issue를 등록함으로써 이루어집니다. 먼저 간략히 Abstract 형태의 Issue 를 등록한 후, 해당 Issue 의 Comment 로 본 튜토리얼을 링크함으로써 제출이 완료됩니다.
* [예시 Issue](https://github.com/PyTorchKR/Tutorial-Competition-2018/issues/1)


1. Abstract 제출 (2018년 11월 30일 (금) 마감)
    - Issue 형태로 등록
    - 제출할 튜토리얼에 대한 간단한 설명
2. 튜토리얼 제출 (2018년 12월 15일 (토) 마감)
    - 웹에 튜토리얼 개재
    - docker image 생성
    - Abstract Issue 의 Comment 로 튜토리얼 및 docker image 링크
    - 마감일 후에는 제출한 튜토리얼 / 이미지 및 Issue 수정 불가


## 일정

1. 2018년 10월 9일 (화): Tutorial Competition 시작
2. 2018년 11월 30일 (금): Abstract 등록 마감
3. 2018년 12월 15일 (토): 튜토리얼 접수 마감
4. 2019년 1월 6일 (일): 수상자 발표
5. 2019년 1월 19일 (토): PyTorch KR Developer Conference


## 상품

- Best Tutorial Award (1팀)
	- [NVIDIA Titan XP](https://www.nvidia.com/ko-kr/titan/titan-xp/)
	    - 2018 CVPR VQA Challenge Runners-up 부상
	    - Jin-Hwa Kim (SK T-Brain), Jaehyun Jun (SNU) and Byoung-Tak Zhang (SNU) 팀에서 기증해 주셨습니다.
	- PyTorch KR DevCon 2018 에서 튜토리얼 진행
- Runner-Up (2~3팀)
	- 20만원 상당의 키보드
	- PyTorch KR DevCon 2018 에서 튜토리얼 진행
	
## 심사위원

- Jin-Hwa Kim (SK T-Brain)
- Tae Yoon Kim (SK T-Brain)
- Hwalsuk Lee (NAVER Clova)
- Nako Sung (NAVER Clova)
- Yunjey Choi (NAVER Clova)
- Keon Kim (Uber)
- Taehoon Kim (OpenAI)
- Sungbin Lim (KakaoBrain)

## FAQ

1. 분량 제한은 없나요?
    - Abstract 은 [예시 Issue](https://github.com/PyTorchKR/Tutorial-Competition-2018/issues/1) 를 참고하여 간결하게 작성해주시면 됩니다.
    - 튜토리얼의 분량에 대한 제한은 따로 없습니다.

## 주최
<a href="https://www.facebook.com/groups/PyTorchKR/"><img src="https://avatars2.githubusercontent.com/u/35714100?s=400&u=8b7264f80c745a0b5ece8bede452ea50e09d6d65&v=4" alt="drawing" width="200"/></a>

<meta property="og:image" content="https://avatars2.githubusercontent.com/u/35714100?s=400&u=8b7264f80c745a0b5ece8bede452ea50e09d6d65&v=4" />


## 문의
- Email: pytorchkr@gmail.com
