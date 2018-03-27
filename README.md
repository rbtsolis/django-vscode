# Django support for Visual Studio Code

Slack Chat:
https://django-vscode.slack.com/

## Overview

## Installation Mode

1. clone this repo

 - go to folder inside the repo
 - You nedd install npm first
 - type in terminal: npm install vsce -g
 - type in terminal: vsce package
 - now you see .vsix file, open this in "Extensions" in Visual Studio Code

or, more simple

2. Go to "Extensions" in Visual Studio Code and search "django visual studio code"

## Snippets for Django templates

| Abbreviation |                     Tag                            |
|--------------|----------------------------------------------------|
| autoescape   |   ``{% autoescape %} {% autoescape %}``            |
| block        |   ``{% block %} {% endblock %}``                   |
| comment      |   ``{% comment %} {% endcomment %}``               |
| csrf         |   ``{% csrf_token %}``                             |
| cycle        |   ``{% cycle %}``                                  |
| debug        |   ``{% debug %}``                                  |
| ext          |   ``{% extends "" %}``                             |
| extends      |   ``{% extends "" %}``                             |
| filter       |   ``{% filter %} {% endfilter %}``                 |
| firstof      |   ``{% firstof %}``                                |
| for          |   ``{% for in %} {% endfor %}``                    |
| fore         |   ``{% for in %} {% empty %} {% endfor %}``        |
| if           |   ``{% if %} {% endif %}``                         |
| ifchanged    |   ``{% ifchanged %} {% endifchanged %}``           |
| ife          |   ``{% if %} {% else %} {% endif %}``              |
| ifelse       |   ``{% if %} {% else %} {% endif %}``              |
| ifeq         |   ``{% ifequal %} {% endifequal %}``               |
| ifequal      |   ``{% ifequal %} {% endifequal %}``               |
| ifnotequal   |   ``{% ifnotequal %} {% endifnotequal %}``         |
| inc          |   ``{% include %}``                                |
| include      |   ``{% include %}``                                |
| load         |   ``{% load %}``                                   |
| now          |   ``{% now "" %}``                                 |
| regroup      |   ``{% regroup by as %}``                          |
| spaceless    |   ``{% spaceless %} {% endspaceless %}``           |
| ssi          |   ``{% ssi %}``                                    |
| static       |   ``{% static %}``                                 |
| templatetag  |   ``{% templatetag %}``                            |
| url          |   ``{% url %}``                                    |
| verbatim     |   ``{% verbatim %} {% endverbatim %}``             |
| widthratio   |   ``{% widthratio %}``                             |
| with         |   ``{% with as %} {% endwith %}``                  |
| trans        |   ``{% trans %}``                                  |
| blocktrans	 |	 ``{% blocktrans with as %} {% endblocktrans %}`` |

...and some non-official stuff:

| Abbreviation |                     Tag                            |
|--------------|----------------------------------------------------|
| super        | `{{ block.super }}`                                |
| extrahead    | `{% block extrahead %} {% endblock extrahead %}`   |
| extrastyle   | `{% block extrastyle %} {% endblock extrastyle %}` |
| var          | `{{ }}`                                            |
| tag          | `{% %}`                                            |
| staticu      | `{{ STATIC_URL }}`                                 |
| media        | `{{ MEDIA_URL }}`                                  |


## Snippets for Django Form 

|  Abbreviation  |  Type  |                        Code - Description                         |
| -------------- | ------ | ----------------------------------------------------------------- |
| Form           | class  | ``Form(with TODOs)``                                              |
| ModelForm      | class  | ``ModelFom``                                                      |
| fbool          | field  | ``forms.BooleanField()``                                          |
| fchar          | field  | ``forms.CharField()``                                             |
| fchoice        | field  | ``forms.ChoiceField()``                                           |
| fcombo         | field  | ``forms.ComboField()``                                            |
| fdate          | field  | ``forms.DateField()``                                             |
| fdatetime      | field  | ``forms.DateTime()``                                              |
| fdecimal       | field  | ``forms.DecimalField()``                                          |
| fduration      | field  | ``forms.DurationField()``                                         |
| femail         | field  | ``forms.EmailField()``                                            |
| ffile          | field  | ``forms.FileField()``                                             |
| ffilepath      | field  | ``forms.FilePathField()``                                         |
| ffloat         | field  | ``forms.FloatField()``                                            |
| fimg           | field  | ``forms.ImageField()``                                            |
| fint           | field  | ``forms.IntegerField()``                                          |
| fip            | field  | ``forms.IPAddressField() - deprecated since version 1.7 ``        |
| fgenericip     | field  | ``forms.GenericIPAddressField()``                                 |
| fmochoice      | field  | ``forms.ModelChoiceField()``                                      |
| fmomuchoice    | field  | ``forms.ModelMultipleChoiceField()``                              |
| fmuchoice      | field  | ``forms.MultipleChoiceField()``                                   |
| ftypedmuchoice | field  | ``forms.TypedMultipleChoiceField()``                              |
| fmuval         | field  | ``forms.MultipleValueField()``                                    |
| fnullbool      | field  | ``forms.NullBooleanField()``                                      |
| fregex         | field  | ``forms.RegexField()``                                            |
| fslug          | field  | ``forms.SlugField()``                                             |
| fsdatetime     | field  | ``forms.SplitDateTime()``                                         |
| ftime          | field  | ``forms.TimeField()``                                             |
| ftchoice       | field  | ``forms.TypedChoiceField()``                                      |
| ftmuchoice     | field  | ``forms.TypedMultipleChoiceField()``                              |
| furl           | field  | ``forms.URLField()``                                              |
| fuuid          | field  | ``forms.UUIDField()``                                             |
| fsimplearray   | field  | ``SimpleArrayField() - PostgreSQL specific form field``           |
| fsplitarray    | field  | ``SplitArrayField() - PostgreSQL specific form field``            |
| fhstore        | field  | ``HStoreField() - PostgreSQL specific form field``                |
| fjson          | field  | ``JSONField() - PostgreSQL specific form field``                  |
| fintrange      | field  | ``IntegerRangeField() - PostgreSQL specific form field``          |
| ffloatrange    | field  | ``FloatRangeField() - PostgreSQL specific form field``            |
| fdatetimerange | field  | ``DateTimeRangeField() - PostgreSQL specific form field``         |
| fdaterange     | field  | ``DateRangeField() - PostgreSQL specific form field``             |
| ffi            | import | ``from .forms import <local_forms>``                         |
| iforms         | import | ``from django import forms``                                      |
| ipostgresff    | import | ``from django.contrib.postgres.forms import <PostgresSQL_forms>`` |
| clean_data     | method | ``validate form data``                                            |

## Snippets for Django model fields

| Abbreviation |                     Tag                            |
|--------------|----------------------------------------------------|
| mauto        | ``models.AutoField()``                            |
| mbigint      | ``models.BigIntegerField()``                      |
| mbool        | ``models.BooleanField()``                         |
| mchar        | ``models.CharField()``                            |
| mcoseint     | ``models.CommaSeparatedIntegerField()``           |
| mdate        | ``models.DateField()``                            |
| mdatetime    | ``models.DateTimeField()``                        |
| mdecimal     | ``models.DecimalField()``                         |
| mduration    | ``models.DurationField()``                        |
| memail       | ``models.EmailField()``                           |
| mfile        | ``models.FileField()``                            |
| mfilepath    | ``models.FilePathField()``                        |
| mfloat       | ``models.FloatField()``                           |
| mimg         | ``models.ImageField()``                           |
| mint         | ``models.IntegerField()``                         |
| mip          | ``models.IPAddressField()``                       |
| mnullbool    | ``models.NullBooleanField()``                     |
| mphone       | ``models.PhoneNumberField()``                     |
| mposint      | ``models.PositiveIntegerField()``                 |
| mpossmallint | ``models.PositiveSmallIntegerField()``            |
| mslug        | ``models.SlugField()``                            |
| msmallint    | ``models.SmallIntegerFiled()``                     |
| mtext        | ``models.TextField()``                             |
| mtime        | ``models.TimeField()``                             |
| murl         | ``models.URLField()``                              |
| musstate     | ``models.USStateField()``                          |
| mxml         | ``models.XMLField()``                              |
| fk           | ``models.ForeignKey()``                            |
| m2m          | ``models.ManyToManyField()``                       |
| o2o          | ``models.OneToOneField()``                         |

## Snippets for Django Rest Framework

|  Abbreviation |                     Tag                            |
|---------------|----------------------------------------------------|
| mserializer   | ``Class for Serialize a Model``                    |
| mviewset      | ``Class for Model ViewSet``                        |
| ronlymviewset | ``Class for ViewSets ReadOnly``                   |

## Snippets for Django Models
|  Abbreviation |                     Tag                            |
|---------------|----------------------------------------------------|
| Model         |     ``Simple Model Class``                         |
| Meta          |     ``Meta Class Django``                          |

## We work hard to add more features for this Extensions, this extension will be updated