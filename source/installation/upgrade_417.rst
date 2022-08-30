#############################
Upgrading from 4.1.6 to 4.1.7
#############################

설치 방법에 해당하는 업그레이드 지침을 참조하십시오.

- :ref:`Composer 설치 - App Starter 업그레이드 <app-starter-upgrading>`
- :ref:`Composer 설치 - 기존 프로젝트의 CodeIgniter4 업그레이드 <adding-codeigniter4-upgrading>`
- :ref:`수동 설치 업그레이드 <installing-manual-upgrading>`

.. contents::
    :local:
    :depth: 2

Breaking Changes
****************

- ``$xssClean``\ 이 true일 때 ``FILTER_SANITIZE_STRING``\ 이 아닌 ``FILTER_SANITIZE_FULL_SPECIAL_CHARS``\ 를 사용하며, 이에 따라 ``get_cookie()``\ 의 출력이 변경됩니다. 변경 사항이 허용 가능한지 확인하십시오. **XSS 필터링**\ 은 XSS 공격을 완벽하게 차단하지는 않으므로, 뷰(view)에서 올바른 ``$context``\ 와 함께 ``esc()``\ 를 사용하기를 권장합니다..