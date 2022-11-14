# TJ-Tasks-2022-abhishek-rai

```py
# Power of 2

def power_of_two(n: int) -> int:
    return 2 ** n

if __name__ == "__main__":
    print(power_of_two(int(input("enter the number:"))))
```

![image](https://user-images.githubusercontent.com/111655497/201627781-4f083f35-0f53-499d-a5e8-6dde48ea519d.png)

---

```py
# Largest Positive Integer That Exists With Its Negative

def find_max_k(nums: list[int]) -> int:
    nums.sort(reverse=True)

    for i in nums:
        if -i in nums:
            return i
    else:
        return -1

if __name__ == "__main__":
    nums = input("Enter the numbers:")
    nums = [int(i) for i in nums.split()]
    print(find_max_k(nums))
```

![image](https://user-images.githubusercontent.com/111655497/201628326-8a45a2c1-6d4c-40ac-b5d1-3c89b58fdfc5.png)

---

```py
# Number of Common Factors

def common_factors(a: int, b: int) -> int:
    small = min(a, b)
    count = 0
    for i in range(1, small + 1):
        if a % i == 0 and b % i == 0:
            count += 1
    return count

if __name__ == "__main__":
    nums = input("Enter two numbers:")
    nums = [int(i) for i in nums.split(" ")]
    print(common_factors(*nums))
```

![image](https://user-images.githubusercontent.com/111655497/201628559-2e98e91a-79cd-46ce-87c5-ee7553c526c8.png)

---

```py
# Maximum 69 Number

def _69(num: int) -> int:
    ls = []
    num_ls = []
    for i in str(num):
        num_ls.append(str(i))

    i = 0
    while i < len(num_ls):
        new_num_list = num_ls.copy()
        if new_num_list[i] == "6":
            new_num_list[i] = "9"
        else:
            new_num_list[i] = "6"
        ls.append(int("".join(new_num_list)))
        i = i + 1

    return max(ls)

if __name__ == "__main__":
    print(_69(int(input("Enter the number:"))))
```

![image](https://user-images.githubusercontent.com/111655497/201628868-e7f0980c-cf89-4e8a-8dc0-553701ac4661.png)

