# pynotebook


cat <<EOF >> $HOME/.bashrc
export PYSPARK_DRIVER_PYTHON=ipython2 # As pyspark only works with python2 and not python3
export PYSPARK_DRIVER_PYTHON_OPTS="notebook"
EOF

cd /dick/pynotebook
jupyter notebook

cd /dick/pynotebook
$SPARK_HOME/bin/pyspark
