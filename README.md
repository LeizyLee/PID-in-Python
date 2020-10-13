# PID-in-Python
PID control in Python  
로봇제어에서 많이 사용되는 PID 제어 모듈입니다.  
PID_control.py의 pid_control 클래스를 사용하며, 객체 생성시 인자값으로 p, i, d 계수를 입력받습니다.  
사용 예시는 파일의 마지막 부분에 있습니다.  

~~~
if __name__ == "__main__":
    pid_controller = pid_control()

    target_value = 5123

    while True:
        pid_controller.pid_calc(target_value)
        print(pid_controller)
        time.sleep(0.01)
~~~
  
