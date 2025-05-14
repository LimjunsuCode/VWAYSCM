이 프로젝트 SCM은 SCM 커밋 기능의 테스트를 위해 작성하였습니다.
커밋 테스트
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    return x / y

print("간단한 계산기입니다.")
print("1. 덧셈\n2. 뺄셈\n3. 곱셈\n4. 나눗셈")

choice = input("원하는 연산을 선택하세요 (1/2/3/4): ")

num1 = float(input("첫 번째 숫자를 입력하세요: "))
num2 = float(input("두 번째 숫자를 입력하세요: "))

if choice == '1':
    print(f"결과: {num1} + {num2} = {add(num1, num2)}")
elif choice == '2':
    print(f"결과: {num1} - {num2} = {subtract(num1, num2)}")
elif choice == '3':
    print(f"결과: {num1} × {num2} = {multiply(num1, num2)}")
elif choice == '4':
    print(f"결과: {num1} ÷ {num2} = {divide(num1, num2)}")
else:
    print("잘못된 입력입니다. 다시 시도해주세요.")
