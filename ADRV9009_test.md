### Dependencies
Install necessary tools
```
pip install -r requirements_dev.txt
```

Build the package
```
python3 setup.py install
```

### Running tests
Running all tests for ADRV9009:
```
/usr/local/lib/python3.8/dist-packages/pyadi_iio-0.0.7-py3.8.egg$ pytest test/test_adrv9009_p.py --custom-hw-map=./adrv9009.yml
```

Running a single test only:
```
filipm@filip-hp850g7:/usr/local/lib/python3.8/dist-packages/pyadi_iio-0.0.7-py3.8.egg$ pytest test/test_adrv9009_p.py --custom-hw-map=./adrv9009.yml -k $TEST_NAME
```
where test name could be any single instance defined in test/test_adrv9009_p.py, e.g. test_adrv9009_dds_gain_check_vary_power, test_adrv9009_dds_gain_check_agc, etc.

