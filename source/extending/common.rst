**************************
공통(common) 기능 교체
**************************

CodeIgniter에 필요한 몇 가지 함수가 핵심(core) 클래스에서 사용하기 위해 초기에 로드되어야 하므로 헬퍼(helper)에 배치할 수 없습니다.
대부분의 사용자는 이 작업을 수행할 필요가 없지만 CodeIgniter 코어를 크게 변경하려는 경우 이러한 기능을 대체할 수 있습니다.
**app/** 디렉토리에는 **Common.php** 파일이 있으며 거기에 정의된 모든 함수는 **system/Common.php**\ 에 있는 버전보다 우선합니다.
또한 프레임워크 전체에서 전역적으로 사용 가능한 기능을 만들 수 있는 기회이기도합니다.

.. note:: 핵심(core) 시스템을 변경하는 것은 프레임워크에 많은 변화를 가져올 수 있음으로, 시도하기 전에 자신이 무엇을 하고 있는지 알아야 합니다.