cmake_minimum_required(VERSION 2.8.3)
project(qt_dotgraph)

find_package(catkin REQUIRED)
catkin_package()

catkin_python_setup()

if (CATKIN_ENABLE_TESTING)
  catkin_add_nosetests(test/pygraphviz_factory_test.py)
  catkin_add_nosetests(test/pydot_factory_test.py)
  catkin_add_nosetests(test/dot_to_qt_test.py)
endif()
