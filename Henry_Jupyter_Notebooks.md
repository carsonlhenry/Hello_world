```python
mkdir /home/student/Desktop/classroom/myfiles/notebooks
```

    mkdir: cannot create directory ‘/home/student/Desktop/classroom/myfiles/notebooks’: File exists



```python
cd /home/student/Desktop/classroom/myfiles/notebooks
```

    /home/student/Desktop/classroom/myfiles/notebooks



```python
sns.set
```




    <function seaborn.rcmod.set(context='notebook', style='darkgrid', palette='deep', font='sans-serif', font_scale=1, color_codes=True, rc=None)>




```python
df=pd.read_csv('/home/student/Desktop/classroom/myfiles/notebooks/fortunee500.csv')
```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    <ipython-input-23-67e6d82e535b> in <module>
    ----> 1 df=pd.read_csv('/home/student/Desktop/classroom/myfiles/notebooks/fortunee500.csv')
    

    ~/anaconda3/lib/python3.7/site-packages/pandas/io/parsers.py in parser_f(filepath_or_buffer, sep, delimiter, header, names, index_col, usecols, squeeze, prefix, mangle_dupe_cols, dtype, engine, converters, true_values, false_values, skipinitialspace, skiprows, skipfooter, nrows, na_values, keep_default_na, na_filter, verbose, skip_blank_lines, parse_dates, infer_datetime_format, keep_date_col, date_parser, dayfirst, cache_dates, iterator, chunksize, compression, thousands, decimal, lineterminator, quotechar, quoting, doublequote, escapechar, comment, encoding, dialect, error_bad_lines, warn_bad_lines, delim_whitespace, low_memory, memory_map, float_precision)
        683         )
        684 
    --> 685         return _read(filepath_or_buffer, kwds)
        686 
        687     parser_f.__name__ = name


    ~/anaconda3/lib/python3.7/site-packages/pandas/io/parsers.py in _read(filepath_or_buffer, kwds)
        455 
        456     # Create the parser.
    --> 457     parser = TextFileReader(fp_or_buf, **kwds)
        458 
        459     if chunksize or iterator:


    ~/anaconda3/lib/python3.7/site-packages/pandas/io/parsers.py in __init__(self, f, engine, **kwds)
        893             self.options["has_index_names"] = kwds["has_index_names"]
        894 
    --> 895         self._make_engine(self.engine)
        896 
        897     def close(self):


    ~/anaconda3/lib/python3.7/site-packages/pandas/io/parsers.py in _make_engine(self, engine)
       1133     def _make_engine(self, engine="c"):
       1134         if engine == "c":
    -> 1135             self._engine = CParserWrapper(self.f, **self.options)
       1136         else:
       1137             if engine == "python":


    ~/anaconda3/lib/python3.7/site-packages/pandas/io/parsers.py in __init__(self, src, **kwds)
       1915         kwds["usecols"] = self.usecols
       1916 
    -> 1917         self._reader = parsers.TextReader(src, **kwds)
       1918         self.unnamed_cols = self._reader.unnamed_cols
       1919 


    pandas/_libs/parsers.pyx in pandas._libs.parsers.TextReader.__cinit__()


    pandas/_libs/parsers.pyx in pandas._libs.parsers.TextReader._setup_parser_source()


    FileNotFoundError: [Errno 2] File b'/home/student/Desktop/classroom/myfiles/notebooks/fortunee500.csv' does not exist: b'/home/student/Desktop/classroom/myfiles/notebooks/fortunee500.csv'



```python
sns.set(style="darkgrid")
```


```python
sns.set(style="darkgrid")
```


```python
/home/student/Desktop/classroom
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-28-0eb218dd1acf> in <module>
    ----> 1 home/student/Desktop/classroom()
    

    NameError: name 'home' is not defined



```python

```
