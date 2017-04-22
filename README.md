# NFSQL, a c++ database operation solution like hibernate.

1) add annotation for class to support scan code for create metadata
2) use metadata to support refletion and class template in c++
3) support connection pool
4) support cache via modifiy metadata configuration
5) support both async query and sync query

Below are the data type that NFSQL should be supported.

int
int64
float
double
std::string
std::vector
std::map
std:list

example1:

@NFSQL_CLASS
class Test
{
public:
  int nTest;
  float fTest;
  std::string strTest;
}

the chart below is the table structure that the class "Test" in database:
