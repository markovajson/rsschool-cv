#  CV Front-end web developer
---
## Personal information & contacts
* Maria Markova
* +7-913-919-37-25, m.markova.wrk@outlook.com
* Discord: Maria Markova (@markovajson)
* [Github](https://github.com/markovajson)
---
*I do yoga and meditation, work with a psychologist on my fears and shortcomings. I love board games, novels, knitting, I read a lot of articles about IT. But my main hobby is my puppy. I give him all my free time: I train, walk, play. And also we travel together and look for new experiences.
I continue to develop myself, I am learning everything new quickly and with pleasure.
I have experience working with Confluence, Jira, Service Desk and MS Office. Basic skills in software testing, HTML/CSS, and C# at the level of writing basic algorithms.*
---
## Skills
* C, C++, C# basics;
* HTML/CSS basics;
* Git;
* Atlassian Jira, Confluence, Service Desk;
* Chrome Devtools;
* MS Office;
* English level B2.
---
## Code example (C#, Dijkstra's algorithm)
        using System;

        namespace AlgorithmD
        {
            class Program 
            {
                static void Swap(ref int a1, ref int a2)
                {

                    var tmp = a1;
                    a1 = a2;
                    a2 = tmp;


                }

                static int[] QuickSort(int[] arr, int minIndex, int maxIndex)
                {

                    if (minIndex >= maxIndex)
                    {

                        return arr;

                    }

                    int pivotIndex = GetPivotIndex(arr, minIndex, maxIndex);

                    QuickSort(arr, minIndex, pivotIndex - 1);

                    QuickSort(arr, pivotIndex + 1, maxIndex);

                    return arr;



                }

                static int GetPivotIndex(int[] arr, int minIndex, int maxIndex)
                {
                    int pivot = minIndex - 1;

                    for (int i = minIndex; i <= maxIndex; i++)
                    {
                        if (arr[i] < arr[maxIndex])
                        {

                            pivot++;
                            Swap(ref arr[pivot], ref arr[i]);

                        }

                    }

                    pivot++;
                    Swap(ref arr[pivot], ref arr[maxIndex]);

                    return pivot;

                }

                static void Main(string[] args)
                {
                    Console.Write("Введите кол-во элементов в ряду: ");
                    int range = Convert.ToInt32(Console.ReadLine());

                    int[] line = new int[range];

                    Console.Write("Введите элементы ряда: ");

                    for (int i = 0; i < range; i++)
                    {
                
                        line[i] = Convert.ToInt32(Console.ReadLine()); 
                        

                    }


                    Console.Write("\n");
                    
                    int j = range - 1;

                    for (int i = range - 1; i >= 0; i--)
                    {
                        if (line[i - 1] >= line[i])
                        {

                            j--;


                        }

                        else
                        {

                            break;

                        }



                    }

                    Console.Write("Первый элемент после хвоста: ");
                    Console.WriteLine(line[j - 1]);

                    Console.Write("\n");
                    
                    int k = range - 1; ;

                    for (int i = range - 1; i >= j - 1; i--)
                    {
                        if (line[i] <= line[j - 1])
                        {

                        k--;


                        }

                        else
                        {

                            Swap(ref line[j - 1], ref line[k]);
                            break;

                        }

                    



                    }

                    Console.Write("Первый элемент после хвоста после обмена: ");
                    Console.WriteLine(line[j - 1]);

                    Console.Write("\n");

                    Console.WriteLine("Перестановка: ");


                    QuickSort(line, j, range - 1);

                    for (int i  = 0; i <= range - 1; i++)
                    {

                        Console.WriteLine(line[i]);


                    }


                }
            }
        }
        
---
## Work experience
* PC operator/Manager (June 2022 - August 2022, RX Group) 
Duties:
processing of requests for documents and customer service.
* PC operator (June 2021 - April 2022, Automatic Technologies)
Duties:
monitoring, testing and analysis of software in industrial operation;
collecting errors during the program and creating tasks for other departments to eliminate them;
maintaining and checking the correctness of reports;
control and processing of incoming information.