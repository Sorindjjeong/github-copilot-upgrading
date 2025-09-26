# upgraded 디렉터리 파일 구조 설명

이 디렉터리는 legacy 프로젝트의 모든 파일과 폴더를 복사하여 최신화 및 포팅 작업을 위한 공간입니다.

## 주요 구조

- `distribute_setup.py`, `distribute-0.6.10.tar.gz`, `MANIFEST.in`, `README.rst`, `setup.py`: 프로젝트 루트의 주요 설정 및 배포 관련 파일
- `docs/`: Sphinx 기반 문서 관련 폴더
    - `Makefile`: 문서 빌드용 Makefile
    - `build/`: 빌드 결과물 (doctrees, html 등)
    - `source/`: 문서 소스(rst, conf.py 등)
- `guachi/`: 주요 Python 모듈 및 서브모듈
    - `__init__.py`, `config.py`, `database.py`: 핵심 모듈 파일
    - `tests/`: 단위 및 통합 테스트 파일
- `guachi.egg-info/`: 패키징 정보 관련 파일
    - `dependency_links.txt`, `PKG-INFO`, `SOURCES.txt`, `top_level.txt`

## 목적
- 모든 legacy 코드를 최신 Python 환경에서 수정, 테스트, 포팅하기 위한 작업 공간
- 원본과 동일한 구조로 복사되어 있어, 각 파일별로 단계적으로 현대화 작업을 진행할 수 있음

---
> 실제 파일 내용은 legacy 폴더에서 복사되어 왔으며, 향후 각 파일별로 Python3 호환성 및 최신 패키징 방식으로 리팩터링이 진행될 예정입니다.
