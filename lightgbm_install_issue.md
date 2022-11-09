## LightGBM 설치 에러 메시지
### 사용한 코드 : pip install lightgbm
### 해결한 코드 : conda install -c conda-forge lightgbm

```
ERROR: Command errored out with exit status 1:
     command: /Users/j-jae0/opt/anaconda3/bin/python -u -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py'"'"'; __file__='"'"'/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' install --record /private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-record-jzmi_e2_/install-record.txt --single-version-externally-managed --compile --install-headers /Users/j-jae0/opt/anaconda3/include/python3.9/lightgbm
         cwd: /private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/
    Complete output (44 lines):
    running install
    /Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    INFO:LightGBM:Starting to compile the library.
    INFO:LightGBM:Starting to compile with CMake.
    Traceback (most recent call last):
      File "/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py", line 95, in silent_call
        subprocess.check_call(cmd, stderr=log, stdout=log)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/subprocess.py", line 368, in check_call
        retcode = call(*popenargs, **kwargs)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/subprocess.py", line 349, in call
        with Popen(*popenargs, **kwargs) as p:
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/subprocess.py", line 951, in __init__
        self._execute_child(args, executable, preexec_fn, close_fds,
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/subprocess.py", line 1821, in _execute_child
        raise child_exception_type(errno_num, err_msg, err_filename)
    FileNotFoundError: [Errno 2] No such file or directory: 'cmake'
    
    During handling of the above exception, another exception occurred:
    
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py", line 334, in <module>
        setup(name='lightgbm',
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/__init__.py", line 87, in setup
        return distutils.core.setup(**attrs)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/_distutils/core.py", line 148, in setup
        return run_commands(dist)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/_distutils/core.py", line 163, in run_commands
        dist.run_commands()
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/_distutils/dist.py", line 967, in run_commands
        self.run_command(cmd)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/dist.py", line 1214, in run_command
        super().run_command(command)
      File "/Users/j-jae0/opt/anaconda3/lib/python3.9/site-packages/setuptools/_distutils/dist.py", line 986, in run_command
        cmd_obj.run()
      File "/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py", line 248, in run
        compile_cpp(use_mingw=self.mingw, use_gpu=self.gpu, use_cuda=self.cuda, use_mpi=self.mpi,
      File "/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py", line 198, in compile_cpp
        silent_call(cmake_cmd, raise_error=True, error_msg='Please install CMake and all required dependencies first')
      File "/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py", line 99, in silent_call
        raise Exception("\n".join((error_msg, LOG_NOTICE)))
    Exception: Please install CMake and all required dependencies first
    The full version of error log was saved into /Users/j-jae0/LightGBM_compilation.log
    ----------------------------------------
ERROR: Command errored out with exit status 1: /Users/j-jae0/opt/anaconda3/bin/python -u -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py'"'"'; __file__='"'"'/private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-install-sq93xc15/lightgbm_73dfb63895624b4cbf0a0a8e75d42724/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' install --record /private/var/folders/2y/wzrmz7495bbdcn9t9svkxxsc0000gn/T/pip-record-jzmi_e2_/install-record.txt --single-version-externally-managed --compile --install-headers /Users/j-jae0/opt/anaconda3/include/python3.9/lightgbm Check the logs for full command output.
```
