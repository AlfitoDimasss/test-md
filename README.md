
# PROGRAMMING & SQL TEST

## 1. Diagonal Difference

Given a square matrix, calculate the absolute difference between the sums of its diagonals.
For example, the square matrix ***arr*** is shown below:

```
1 2 3
4 5 6
9 8 9
```

The left-to-right diagonal = **1 + 5 + 9 = 15**. The right to left diagonal = **3 + 5 + 7 = 15**. Their absolute difference is **|15 - 17| = 2**.

### Function Description

Create the ***diagonalDifference*** function, which takes the following parameter:

**int arr[n][m]**: an array of integers

### Return

- **int**: the absolute diagonal difference

### Input Format

The first line contains a single integer, ***n***, the number of rows and columns in the square matrix ***arr***.
Each of the next ***n*** lines describes a row, ***arr[i]***, and consists of ***n*** space-separated integers ***arr[i][j]***.

### Output Format

Return the absolute difference between the sums of the matrix's two diagonals as a single integer.

### Sample Input

```
3
11 2 4
4 5 6
10 8 -12
```

### Sample Output

```
15
```

## 2. Smart Number

A number is called a smart number if it has an odd number of factors. Given some numbers, find whether they are smart numbers or not.

Create a function called ***is_smart_number*** to correctly check if a given number is a smart number.

### Input Format

The first line of the input contains ***t***, the number of test cases.
The next ***t*** lines contain one integer each.

### Output Format

The output should consist of ***t*** lines. In the ***i*** line print YES if the ***i*** integer has an odd number of factors, else print NO.

### Sample Input

```
4
1
2
7
169
```

### Sample Output
```
YES
NO
NO
YES
```

### Explanation

The factors of 1 are just 1 itself.So the answer is YES. The factors of 2 are 1 and 2.It has even number of factors.The answer is NO. The factors of 7 are 1 and 7.It has even number of factors.The answer is NO. The factors of 169 are 1,13 and 169.It has odd number of factors.The answer is YES.

## 3. Number Line Jumps

You are choreographing a circus show with various animals. For one act, you are given two kangaroos on a number line ready to jump in the positive direction (i.e, toward positive infinity).

- The first kangaroo starts at location ***x1*** and moves at a rate of ***v1*** meters per jump.
- The second kangaroo starts at location ***x2*** and moves at a rate of ***v2*** meters per jump.

You have to figure out a way to get both kangaroos at the same location at the same time as part of the show by creating a function names ***kangaroo***. If it is possible, return YES, otherwise return NO.

### Example

***x1* = 2**\
***v1* = 1**\
***x2* = 1**\
***v2* = 2**

After one jump, they are both at ***x = 3***, (***x1 + v1 = 2 + 1, x2 + v2 = 1 + 2***), so the answer is ```YES```.

### Returns

- string: either ```YES``` or ```No```

### Input Formats

A single line of four space-separated integers denoting the respective values of ***x1***, ***v1***, ***x2***, and ***v2***.

### Constraints

- **0 <= x1 < x2 <= 10000**
- **1 <= v1 <= 10000**
- **1 <= v2 <= 10000**

### Sample Input 1

```
0 3 4 2
```

### Sample Output 1

```
YES
```

### Explanation 1

The two kangaroos jump through the following sequence of locations:

![Kangaroo](https://s3.amazonaws.com/hr-assets/0/1516005283-e74e76ff0c-kangaroo.png)

From the image, it is clear that the kangaroos meet at the same location (number ***12*** on the number line) after same number of jumps (***4*** jumps), and we print YES.

### Sample Input 2

```
0 2 5 3
```

### Sample Output 2

```
NO
```

### Explanation 2

The second kangaroo has a starting location that is ahead (further to the right) of the first kangaroo's starting location (i.e., ***x2 > x1***). Because the second kangaroo moves at a faster rate (meaning ***v2 > v1***) and is already ahead of the first kangaroo, the first kangaroo will never be able to catch up. Thus, we print NO.

# 4. SQL DDL

As a database administrator you are assigned to create a DDL to create the database tables as shown on Physical Data Diagaram below:

![PDD](https://www.gooddata.com/img/blog/_2000xauto/pdm-for-e-commerce.png.webp)

Mandatory Table:
- ***product***
- ***customer***
- ***order_line***

Optional Table:
- ***date***

# 5. SQL DML

Based on the database tables that you've created before, please create SQL DML script to Insert, Update, and Delete based on this scenario:

1. Create customers
```
[
    {
        name: Yanto
        state: India
        region: Kolkata
    },
    {
        name: Wiji
        state: Indonesia
        region: Walantaka
    }
]
```

2. Create products
```
[
    {
        product_name: How to be a Good Father
        category: book
    },
    {
        product_name: Lupis
        category: food
    }
]
```

3. Create orders

```
1. Yanto order single product 1
1. Yanto order 3 pcs of product 2
2. Wiji order 5 pcs of product 2
```

# 6. SQL JOIN

Based on the database tables that you've created before, please create SQL Join table script between customers - order - products table.





