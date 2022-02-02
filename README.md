# 영상 단어장 자동화 스크립트
-----------------------
유튜브 등에는 단어암기를 돕는 많은 영상들이 있습니다. 이런 영상들은 대개 형식은 장시간 유지된 채 내용만 바뀌는 식으로 제작됩니다. 이를 일일이 타이핑하거나 tts를 녹음하여 수작업으로 영상을 제작한다고 하면 굉장히 수고스러운 일일 것입니다. 이 레포지토리는 노가다성 영상 제작에 들어가는 수고를 덜 수 있는 간단한 솔루션을 제공합니다.

## 필요 라이브러리
다음 라이브러리를 pip를 통해 설치해주세요.
* pip install pillow (PIL)
* pip install moviepy
* pip install gtts
* pip install pydub

## 파라미터
콘솔에 다음의 간단한 파라미터만 넣어주면 자동으로 영상을 제작할 수 있습니다.
> filmer.py words.txt photo.jpg

#### words.txt
제작하고자 하는 단어의 리스트입니다. 토큰은 '|'로 구분되고 좌항은 단어, 우항은 그 단어의 의미입니다. 사용자가 메모장으로 손수 제작할 수도 있겠으나 저 같은 경우에는 'Quizlet'에서 단어장을 만들고 그곳에서 Export하는 방식을 사용합니다.
#### photo.jpg
단어장의 뒷배경입니다. 세로 사진의 경우 단어 길이에 따라 짤릴 수 있으므로 조정이 필요합니다.

----------------------------
###### 위를 실행시키면 py 스크립트가 있는 디렉토리에 '__resultat.mp4' 파일이 생성됩니다.
###### 이외에 폰트나 폰트 크기 같은 경우 직접 스트립트를 수정하여 커스터마이징하실 수 있습니다.
###### 코드 수정을 통해 tts 언어 설정을 변경할 수 있으나 위 스크립트는 프랑스어-한국어에 최적화되어 있습니다.
