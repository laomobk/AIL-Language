#! /usr/bin/python3

from core import ail_launcher
import sys
import os.path


def init_core_path():
    # init core path

    p = os.path.split(os.path.abspath(__file__))[0]

    cp = os.path.join(p, 'core' + os.path.sep)

    if not os.path.exists(cp) or os.path.isfile(cp):
        print('AIL Error : Cannot init core files !')
        sys.exit(1)

    sys.path.append(cp)


if __name__ == '__main__':
    init_core_path()
    ail_launcher.launch_main(sys.argv[1:])
