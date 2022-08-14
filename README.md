Introduction
This repository contains several Web UI tests for eldorado.ru. Uses PyTest + Selenium.
Files

conftest.py contains all the required code to catch failed test cases and make screenshot of the page in case any test case will fail.

pytest.ini contains driver select and path.

pages/base.py contains PageObject pattern implementation for Python.

pages/eldorado_page.py contains class to define web elements on testing page.

pages/elements.py contains helper class to define web elements on web pages.

pages/helpers.py contains common constants and methods? used in tests.

tests/test_run_1_main_page.py contains several Web UI tests for main page elements.

tests/test_run_2_region_select.py contains several Web UI tests for the region selection functionality.

tests/test_run_3_basket.py contains several Web UI tests for basket page elements.

tests/test_run_4_search_and_filtering.py contains several Web UI tests for search and filtering functionality.
How To Run Tests

    Install all requirements:

    pip3 install -r requirements.txt

    Download and unpack Selenium WebDriver (choose version which is compatible with your browser).

    Open conftest.py and specify the driver type and path to the executable file.

    Run tests:

    python -m pytest -v tests/
