{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNKj0Y1P8fSFZzIGU1VGLxX",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/MatthewLieberman0/BTE320-InClassAssignmentss/blob/main/README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": 2,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "yE4ImuuZCmQH",
        "outputId": "8a90c176-71ad-4bff-ae1b-c3ff60745d60"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "244.92000000000002\n"
          ]
        }
      ],
      "source": [
        "h = 10\n",
        "r = 3\n",
        "pi = 3.14\n",
        "SurfaceArea = (2 * pi * r ** 2) + (2 * pi * r * h)\n",
        "\n",
        "print(SurfaceArea)\n",
        "\n"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "import random\n",
        "\n",
        "choice = input('Do you want to play a game?')\n",
        "while choice == 'yes':\n",
        "  p1 = input('Choose rock, paper, or scissors')\n",
        "  p2 = random.choice(['rock', 'paper', 'scissors'])\n",
        "  print(f'Computer chose {p2}.')\n",
        "  if p1 == p2:\n",
        "    print('Draw')\n",
        "  elif p1 == 'rock' and p2 == 'scissors':\n",
        "   print('p1 wins')\n",
        "  elif p1 == 'paper' and p2 == 'rock':\n",
        "    print('p1 wins')\n",
        "  elif p1 == 'scissors' and p2 == 'paper':\n",
        "    print('p1 wins')\n",
        "  else:\n",
        "    print('p2 wins')\n",
        "  choice = input('Do you want to play a game?')"
      ],
      "metadata": {
        "id": "J5TmmJK8mjs2"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "n1 = float(input('Choose the first number'))\n",
        "n2 = float(input('Choose the second number'))\n",
        "symbol = input('Choose the symbol for calculation (+, -, *, /, **)')\n",
        "\n",
        "if symbol == '+':\n",
        "  print(n1 + n2)\n",
        "elif symbol == '-':\n",
        "  print(n1 - n2)\n",
        "elif symbol == '*':\n",
        "  print(n1*n2)\n",
        "elif symbol == '/':\n",
        "  print(n1/n2)\n",
        "elif symbol == '**':\n",
        "  print(n1**n2)"
      ],
      "metadata": {
        "id": "BQTTutTlWvOO",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "ad2af0a8-d96e-48e0-f951-4ddc77d2619c"
      },
      "execution_count": 6,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Choose the first number1\n",
            "Choose the second number8\n",
            "Choose the symbol for calculation (+, -, *, /, **)*\n",
            "8.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "flatRate = 5\n",
        "hourlyRate = 2.5\n",
        "\n",
        "for hour in range(1, 9, 1):\n",
        "  charge = flatRate + hourlyRate * hour\n",
        "  if charge < 10:\n",
        "    charge = 10.0\n",
        "  elif charge > 20:\n",
        "    charge = 20.0\n",
        "  print(hour, ' ', charge)\n",
        "\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "collapsed": true,
        "id": "YW35TLRdaS-r",
        "outputId": "355854e7-7173-45d8-df3f-c775e9391d47"
      },
      "execution_count": 7,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1   10.0\n",
            "2   10.0\n",
            "3   12.5\n",
            "4   15.0\n",
            "5   17.5\n",
            "6   20.0\n",
            "7   20.0\n",
            "8   20.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def calcFree(hours):\n",
        "   float(input('Enter hours parked: '))\n",
        "\n",
        "hours = float(input('Enter hours parked: '))\n",
        "c = (5 + hours*2.5)\n",
        "print(c)\n",
        "\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "tiAbnF9DcNMO",
        "outputId": "cf5f8cb6-3f83-4ce1-e8f2-9420f24b3fbe"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter hours parked: 4\n",
            "15.0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for ad in range(0, 201, 25):\n",
        "  additional = 2*round(ad**.5)\n",
        "  profit = ((20 + additional) * 10) - 200 - ad\n",
        "  print(ad, ' ', profit)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "D-IVNTvykoJw",
        "outputId": "f6004287-d7d4-4219-b87a-eb7ed1c22591"
      },
      "execution_count": 8,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0   0\n",
            "25   75\n",
            "50   90\n",
            "75   105\n",
            "100   100\n",
            "125   95\n",
            "150   90\n",
            "175   85\n",
            "200   80\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "months = {}\n",
        "\n",
        "names = [\"Jan\", \"Feb\", \"Mar\", \"Apr\", \"May\", \"Jun\", \"Jul\", \"Aug\", \"Sep\", \"Oct\", \"Nov\", \"Dec\"]\n",
        "numbers = [1,2,3,4,5,6,7,8,9,10,11,12]\n",
        "\n",
        "for i in numbers:\n",
        "  months[i] = names[i-1]\n",
        "months"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ta3mNoMfaduB",
        "outputId": "867ac0f7-c0ce-45ef-b75c-88d5ee71782c"
      },
      "execution_count": 9,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "{1: 'Jan',\n",
              " 2: 'Feb',\n",
              " 3: 'Mar',\n",
              " 4: 'Apr',\n",
              " 5: 'May',\n",
              " 6: 'Jun',\n",
              " 7: 'Jul',\n",
              " 8: 'Aug',\n",
              " 9: 'Sep',\n",
              " 10: 'Oct',\n",
              " 11: 'Nov',\n",
              " 12: 'Dec'}"
            ]
          },
          "metadata": {},
          "execution_count": 9
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "months = {}\n",
        "\n",
        "names = [\"Jan\", \"Feb\", \"Mar\", \"Apr\", \"May\", \"Jun\", \"Jul\", \"Aug\", \"Sep\", \"Oct\", \"Nov\", \"Dec\"]\n",
        "numbers = [1,2,3,4,5,6,7,8,9,10,11,12]\n",
        "\n",
        "for i in range(len(numbers)):\n",
        "  months[numbers[i]] = names[i]\n",
        "months\n",
        "\n",
        "\n",
        "\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jyEo80PGWGkL",
        "outputId": "b9319316-0163-4f1e-d382-1fef1d558934"
      },
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "{1: 'Jan',\n",
              " 2: 'Feb',\n",
              " 3: 'Mar',\n",
              " 4: 'Apr',\n",
              " 5: 'May',\n",
              " 6: 'Jun',\n",
              " 7: 'Jul',\n",
              " 8: 'Aug',\n",
              " 9: 'Sep',\n",
              " 10: 'Oct',\n",
              " 11: 'Nov',\n",
              " 12: 'Dec'}"
            ]
          },
          "metadata": {},
          "execution_count": 10
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "for value in months.values():\n",
        "  print(value)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "LyjAO2MrhPr_",
        "outputId": "a5d72b72-9795-4c1a-b1cb-473ed8f86ec8"
      },
      "execution_count": 11,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Jan\n",
            "Feb\n",
            "Mar\n",
            "Apr\n",
            "May\n",
            "Jun\n",
            "Jul\n",
            "Aug\n",
            "Sep\n",
            "Oct\n",
            "Nov\n",
            "Dec\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def calcFee(hours, decimals=2):\n",
        "  fee = round(5 + hours*2.5, decimals)\n",
        "  return fee\n",
        "def displayFee(fee):\n",
        "  print(fee)\n",
        "\n",
        "h = int(input('Enter hours for parking: '))\n",
        "f = calcFee(h)\n",
        "displayFee(f)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "G06mz9JSgKMF",
        "outputId": "8ba42949-6d58-40d6-85e1-d8b57d2d9f6f"
      },
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter hours for parking: 5\n",
            "17.5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def rev(s):\n",
        "  if len(s)==1:\n",
        "    return s\n",
        "  else:\n",
        "    return rev(s[1:]) + s[0]\n",
        "\n",
        "rev('Hello')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "id": "mSDn6OdCkeqj",
        "outputId": "4d2a1c76-7dfd-4077-c2bc-11916389805d"
      },
      "execution_count": 13,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "'olleH'"
            ],
            "application/vnd.google.colaboratory.intrinsic+json": {
              "type": "string"
            }
          },
          "metadata": {},
          "execution_count": 13
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "def wAvg(L, W):\n",
        "  try:\n",
        "    res = []\n",
        "    for i in range(len(L)):\n",
        "      res.append(L[i] * W[i])\n",
        "    return sum(res) / sum(W)\n",
        "  except ZeroDivisionError:\n",
        "    print('Division by zero')\n",
        "    return []\n",
        "  except TypeError:\n",
        "    print('Non-numerical objects found')\n",
        "    return []\n",
        "  except Exception as e:\n",
        "    print(f'Unknown error: {e}')\n",
        "    return float('nan')\n",
        "\n",
        "wAvg([1,2,3], [0.1, 0.3, 0.4])"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "bqWfYyXq9jO1",
        "outputId": "6743ad39-c66d-41b7-fa8b-1e8052f32f8a"
      },
      "execution_count": 14,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "2.375"
            ]
          },
          "metadata": {},
          "execution_count": 14
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "  def __init__ (self, name, number):\n",
        "    self.name = name\n",
        "    self.number = number\n",
        "\n",
        "  def __str__(self):\n",
        "    return f'Name: {self.name}.'"
      ],
      "metadata": {
        "id": "VjNdt-qE2thU"
      },
      "execution_count": 15,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "s1 = Student('James Bond', '007')\n",
        "s2 = Student('Clark Kent', '333')"
      ],
      "metadata": {
        "id": "6MenpQ-03pfx"
      },
      "execution_count": 16,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "print(s1)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eVlwv4ku4Byg",
        "outputId": "5f5369a0-a10b-4e04-f3d5-4db9440c0b0e"
      },
      "execution_count": 17,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: James Bond.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "class Student:\n",
        "  def __init__(self, name, number):\n",
        "    self.name = name\n",
        "    self.number = number\n",
        "    self.__courses = []\n",
        "\n",
        "  def enroll(self,course):\n",
        "    if course not in self.__courses:\n",
        "      self.__courses.append(course)\n",
        "    else:\n",
        "      print(f'You have already enrolled in course: {course}')\n",
        "\n",
        "  def get_courses(self):\n",
        "    return self.__courses\n",
        "\n",
        "\n",
        "s = Student('Bob', '123')\n",
        "s.enroll('ABC123')\n",
        "s.enroll('ABC456')\n",
        "s.enroll('ABC789')\n",
        "s.get_courses()\n",
        "s.enroll('ABC123')\n",
        "\n",
        "# s.__courses.append('ABC123') (that will give you an error)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ld3BgsI28H1e",
        "outputId": "18c0abd3-bca2-4b46-bcbb-b83ad12d6441"
      },
      "execution_count": 18,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "You have already enrolled in course: ABC123\n"
          ]
        }
      ]
    }
  ]
}