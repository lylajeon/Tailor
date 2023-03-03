# 2022-1 소프트웨어종합설계 Tailor 팀

- Presentation 
  - video: [link](https://youtu.be/6ecoxuVkcSE)
  - pdf: [link](https://github.com/lylajeon/Tailor/blob/main/presentation.pdf)
  - code for mobile app: [link](https://github.com/KyooSikLee/Tailor)

- ./STAR
  - STAR 와 관련된 코드입니다.
  - ./STAR/model/star_1_1/male/model.npz 를 https://drive.google.com/file/d/1N66BUShOyoHhFGZwCaHJawuvI7t4K39z/view?usp=sharing 에서 다운받으세요.
  - ./STAR/model/neutral_smpl_with_cocoplus_reg.txt 를 https://drive.google.com/file/d/1N8ZzrWPeX7TXUGiBF8yiuMHWvcYKCCXl/view?usp=sharing 에서 다운받으세요.

- ./ClothingShapePoseModel
  - shape, pose -> cloth vertices
  - clothing_shape_model.py
    - AgentDress 의 clothing shape model 을 구현해본 코드입니다. 사용하지는 않을 거 같지만 일단 남겨뒀습니다.
  - clothing_shape_pose_model.py
    - main 코드 입니다.
  - mlp.py
    - training 과 관련된 코드들입니다.
  - models.py
    - clothing shape pose model 의 몸체입니다. 아랫쪽에 deprecate 되었다고 써놓은 코드들은 AgentDress 의 clothing shape model 인데, 역시 사용하진 않겠지만 일단 남겨뒀습니다.
  - utils.py
    - 기타 obj 파일을 로드하거나 save 하는 등의 코드들입니다.
  - 사용법!!
    - ./ClothingShapePoseModel/settings/setting1.yml 을 생성해주세요. (예시: https://drive.google.com/file/d/1N1CV5nasU00FvC3QpcTd0ux56-DaUMX8/view?usp=sharing)
    - yml 내부의 base_body_dir 을 데이터셋의 디렉토리로 바꿔주세요.
    - 처음 실행 시에는 train 을 True 로 해주세요.
    - ./ClothingShapePoseModel/model 디렉토리를 생성해주세요.
    - root 디렉토리의 이름은 sojong 이어야 합니다.
    - pytorch 등 필요한 라이브러리가 설치되어있어야 합니다.
    - `python clothing_shape_pose_model.py`
