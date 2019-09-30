--
-- PostgreSQL database cluster dump
--

-- Started on 2019-09-30 16:33:03 PST

SET default_transaction_read_only = off;

SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;

--
-- Roles
--

CREATE ROLE brem;
ALTER ROLE brem WITH SUPERUSER INHERIT NOCREATEROLE NOCREATEDB LOGIN NOREPLICATION NOBYPASSRLS PASSWORD 'md5e5fbfdd65b01da6d53a7bdd020c18d79';
CREATE ROLE brem2;
ALTER ROLE brem2 WITH SUPERUSER INHERIT NOCREATEROLE NOCREATEDB LOGIN NOREPLICATION NOBYPASSRLS PASSWORD 'md5b6d2e688d25b39d305d1d366aa1c93ed';
CREATE ROLE patrick;
ALTER ROLE patrick WITH SUPERUSER INHERIT NOCREATEROLE NOCREATEDB LOGIN NOREPLICATION NOBYPASSRLS PASSWORD 'md5b17a8f54ae984922b1b8c77b7b188085';
CREATE ROLE postgres;
ALTER ROLE postgres WITH SUPERUSER INHERIT CREATEROLE CREATEDB LOGIN REPLICATION BYPASSRLS;






--
-- Database creation
--

CREATE DATABASE "180000000297" WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE barcelo__week8_project WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE barcelo_week10 WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE barcelo_week8_select WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE brem WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE ima WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE mydb WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE store WITH TEMPLATE = template0 OWNER = postgres;
REVOKE CONNECT,TEMPORARY ON DATABASE template1 FROM PUBLIC;
GRANT CONNECT ON DATABASE template1 TO PUBLIC;
CREATE DATABASE week10 WITH TEMPLATE = template0 OWNER = postgres;
CREATE DATABASE workgroup WITH TEMPLATE = template0 OWNER = postgres;


\connect "180000000297"

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:03 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2906 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


-- Completed on 2019-09-30 16:33:04 PST

--
-- PostgreSQL database dump complete
--

\connect barcelo__week8_project

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:04 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2906 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


-- Completed on 2019-09-30 16:33:05 PST

--
-- PostgreSQL database dump complete
--

\connect barcelo_week10

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:05 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 9 (class 2615 OID 41069)
-- Name: barcelo_problem5a; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA barcelo_problem5a;


ALTER SCHEMA barcelo_problem5a OWNER TO postgres;

--
-- TOC entry 10 (class 2615 OID 41076)
-- Name: barcelo_problem5b; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA barcelo_problem5b;


ALTER SCHEMA barcelo_problem5b OWNER TO postgres;

--
-- TOC entry 7 (class 2615 OID 41083)
-- Name: barcelo_problem5c; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA barcelo_problem5c;


ALTER SCHEMA barcelo_problem5c OWNER TO postgres;

--
-- TOC entry 8 (class 2615 OID 41048)
-- Name: barcelo_problem6a; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA barcelo_problem6a;


ALTER SCHEMA barcelo_problem6a OWNER TO postgres;

--
-- TOC entry 4 (class 2615 OID 41062)
-- Name: barcelo_problem6b; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA barcelo_problem6b;


ALTER SCHEMA barcelo_problem6b OWNER TO postgres;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2970 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 207 (class 1259 OID 41073)
-- Name: studassistant; Type: TABLE; Schema: barcelo_problem5a; Owner: postgres
--

CREATE TABLE barcelo_problem5a.studassistant (
    sa_fname character varying(20) NOT NULL,
    sa_lname character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5a.studassistant OWNER TO postgres;

--
-- TOC entry 206 (class 1259 OID 41070)
-- Name: student; Type: TABLE; Schema: barcelo_problem5a; Owner: postgres
--

CREATE TABLE barcelo_problem5a.student (
    s_name character varying(20) NOT NULL,
    s_lname character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5a.student OWNER TO postgres;

--
-- TOC entry 208 (class 1259 OID 41077)
-- Name: studassistant; Type: TABLE; Schema: barcelo_problem5b; Owner: postgres
--

CREATE TABLE barcelo_problem5b.studassistant (
    sa_fname character varying(20) NOT NULL,
    sa_lname character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5b.studassistant OWNER TO postgres;

--
-- TOC entry 209 (class 1259 OID 41080)
-- Name: student; Type: TABLE; Schema: barcelo_problem5b; Owner: postgres
--

CREATE TABLE barcelo_problem5b.student (
    s_fname character varying(20) NOT NULL,
    s_lname character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5b.student OWNER TO postgres;

--
-- TOC entry 211 (class 1259 OID 41087)
-- Name: outcomes; Type: TABLE; Schema: barcelo_problem5c; Owner: postgres
--

CREATE TABLE barcelo_problem5c.outcomes (
    ship character varying(20) NOT NULL,
    battle character varying(20) NOT NULL,
    result character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5c.outcomes OWNER TO postgres;

--
-- TOC entry 210 (class 1259 OID 41084)
-- Name: ships; Type: TABLE; Schema: barcelo_problem5c; Owner: postgres
--

CREATE TABLE barcelo_problem5c.ships (
    name character varying(20) NOT NULL,
    class character varying(20) NOT NULL,
    launched character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem5c.ships OWNER TO postgres;

--
-- TOC entry 202 (class 1259 OID 41054)
-- Name: product; Type: TABLE; Schema: barcelo_problem6a; Owner: postgres
--

CREATE TABLE barcelo_problem6a.product (
    p_code numeric(6,0) NOT NULL,
    p_descript character varying(20) NOT NULL,
    price character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem6a.product OWNER TO postgres;

--
-- TOC entry 203 (class 1259 OID 41059)
-- Name: store; Type: TABLE; Schema: barcelo_problem6a; Owner: postgres
--

CREATE TABLE barcelo_problem6a.store (
    store numeric(2,0) NOT NULL,
    angle character varying(5) NOT NULL,
    shelf numeric(1,0) NOT NULL
);


ALTER TABLE barcelo_problem6a.store OWNER TO postgres;

--
-- TOC entry 201 (class 1259 OID 41049)
-- Name: student; Type: TABLE; Schema: barcelo_problem6a; Owner: postgres
--

CREATE TABLE barcelo_problem6a.student (
    p_code numeric(6,0) NOT NULL,
    p_descript character varying(20) NOT NULL,
    price character varying(20) NOT NULL
);


ALTER TABLE barcelo_problem6a.student OWNER TO postgres;

--
-- TOC entry 204 (class 1259 OID 41063)
-- Name: t1; Type: TABLE; Schema: barcelo_problem6b; Owner: postgres
--

CREATE TABLE barcelo_problem6b.t1 (
    label character varying(1) NOT NULL
);


ALTER TABLE barcelo_problem6b.t1 OWNER TO postgres;

--
-- TOC entry 205 (class 1259 OID 41066)
-- Name: t2; Type: TABLE; Schema: barcelo_problem6b; Owner: postgres
--

CREATE TABLE barcelo_problem6b.t2 (
    score numeric(1,0) NOT NULL
);


ALTER TABLE barcelo_problem6b.t2 OWNER TO postgres;

--
-- TOC entry 2958 (class 0 OID 41073)
-- Dependencies: 207
-- Data for Name: studassistant; Type: TABLE DATA; Schema: barcelo_problem5a; Owner: postgres
--

COPY barcelo_problem5a.studassistant (sa_fname, sa_lname) FROM stdin;
Franklin	Lopez
William	Turner
Franklin	Johnson
Susan	Rogers
\.


--
-- TOC entry 2957 (class 0 OID 41070)
-- Dependencies: 206
-- Data for Name: student; Type: TABLE DATA; Schema: barcelo_problem5a; Owner: postgres
--

COPY barcelo_problem5a.student (s_name, s_lname) FROM stdin;
George	Jones
Jane	Smith
Peter	Robinson
Franklin	Johnson
Martin	Lopez
\.


--
-- TOC entry 2959 (class 0 OID 41077)
-- Dependencies: 208
-- Data for Name: studassistant; Type: TABLE DATA; Schema: barcelo_problem5b; Owner: postgres
--

COPY barcelo_problem5b.studassistant (sa_fname, sa_lname) FROM stdin;
Franklin	Lopez
William	Turner
Franklin	Johnson
Susan	Rogers
\.


--
-- TOC entry 2960 (class 0 OID 41080)
-- Dependencies: 209
-- Data for Name: student; Type: TABLE DATA; Schema: barcelo_problem5b; Owner: postgres
--

COPY barcelo_problem5b.student (s_fname, s_lname) FROM stdin;
George	Jones
Jane	Smith
Peter	Robinson
Franklin	Johnson
Martin	Lopez
\.


--
-- TOC entry 2962 (class 0 OID 41087)
-- Dependencies: 211
-- Data for Name: outcomes; Type: TABLE DATA; Schema: barcelo_problem5c; Owner: postgres
--

COPY barcelo_problem5c.outcomes (ship, battle, result) FROM stdin;
Bismarck	North Atlantic	sunk
California	Guadalcanal	damaged
California	Surigao Strait	OK
Duke of York	North Cape	OK
Fuso	Surigao Strait	sunk
Hood	North Atlantic	sunk
King George V	North Atlantic	OK
Kirishima	Guadalcanal	sunk
Prince of Wales	North Atlantic	damaged
Rodney	North Atlantic	OK
Schamhorst	North Cape	sunk
South Dakota	Guadalcanal	damaged
Tennessee	Surigao Strait	OK
Washington	Guadalcanal	OK
West Virginia	Surigao Strait	OK
Yamashiro	Surigao Strait	sunk
\.


--
-- TOC entry 2961 (class 0 OID 41084)
-- Dependencies: 210
-- Data for Name: ships; Type: TABLE DATA; Schema: barcelo_problem5c; Owner: postgres
--

COPY barcelo_problem5c.ships (name, class, launched) FROM stdin;
California	Tennessee	1921
Haruna	Kongo	1916
Hiei	Kongo	1914
Iowa	Iowa	1943
Kirishima	Kongo	1915
Kongo	Kongo	1913
Missouri	Iowa	1944
Musashi	Yamato	1942
New Jersey	Iowa	1943
North Carolina	North Carolina	1941
Ramillies	Revenge	1917
Renown	Renown	1916
Repulse	Renown	1916
Resolution	Renown	1916
Revenge	Revenge	1916
Royal Oak	Revenge	1916
Royal Sovereign	Revenge	1916
South Dakota	North Carolina	1941
Tennessee	Tennessee	1920
Washington	North Carolina	1941
Wisconsin	Iowa	1944
Yamato	Yamato	1941
\.


--
-- TOC entry 2953 (class 0 OID 41054)
-- Dependencies: 202
-- Data for Name: product; Type: TABLE DATA; Schema: barcelo_problem6a; Owner: postgres
--

COPY barcelo_problem6a.product (p_code, p_descript, price) FROM stdin;
123456	Flasghlight	5.26
123457	lamp	25.15
123458	Box fan	10.99
213345	9v Battery	1.92
254467	100W bulb	1.47
311452	powerdrill	34.99
\.


--
-- TOC entry 2954 (class 0 OID 41059)
-- Dependencies: 203
-- Data for Name: store; Type: TABLE DATA; Schema: barcelo_problem6a; Owner: postgres
--

COPY barcelo_problem6a.store (store, angle, shelf) FROM stdin;
23	W	5
24	K	9
25	Z	6
\.


--
-- TOC entry 2952 (class 0 OID 41049)
-- Dependencies: 201
-- Data for Name: student; Type: TABLE DATA; Schema: barcelo_problem6a; Owner: postgres
--

COPY barcelo_problem6a.student (p_code, p_descript, price) FROM stdin;
\.


--
-- TOC entry 2955 (class 0 OID 41063)
-- Dependencies: 204
-- Data for Name: t1; Type: TABLE DATA; Schema: barcelo_problem6b; Owner: postgres
--

COPY barcelo_problem6b.t1 (label) FROM stdin;
A
B
\.


--
-- TOC entry 2956 (class 0 OID 41066)
-- Dependencies: 205
-- Data for Name: t2; Type: TABLE DATA; Schema: barcelo_problem6b; Owner: postgres
--

COPY barcelo_problem6b.t2 (score) FROM stdin;
1
2
3
\.


--
-- TOC entry 2830 (class 2606 OID 41058)
-- Name: product product_pkey; Type: CONSTRAINT; Schema: barcelo_problem6a; Owner: postgres
--

ALTER TABLE ONLY barcelo_problem6a.product
    ADD CONSTRAINT product_pkey PRIMARY KEY (p_code);


--
-- TOC entry 2828 (class 2606 OID 41053)
-- Name: student student_pkey; Type: CONSTRAINT; Schema: barcelo_problem6a; Owner: postgres
--

ALTER TABLE ONLY barcelo_problem6a.student
    ADD CONSTRAINT student_pkey PRIMARY KEY (p_code);


-- Completed on 2019-09-30 16:33:06 PST

--
-- PostgreSQL database dump complete
--

\connect barcelo_week8_select

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:06 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2911 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 196 (class 1259 OID 40969)
-- Name: p1a; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.p1a (
    p_code numeric(6,0) NOT NULL,
    p_descript character varying(20) NOT NULL,
    p_price numeric(4,2) NOT NULL
);


ALTER TABLE public.p1a OWNER TO postgres;

--
-- TOC entry 2903 (class 0 OID 40969)
-- Dependencies: 196
-- Data for Name: p1a; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.p1a (p_code, p_descript, p_price) FROM stdin;
123456	flashlight	5.26
123457	lamp	25.15
123458	Box fan	10.99
213345	9v Battery	1.92
254467	100W bulb	1.47
311452	powerdrill	34.99
\.


-- Completed on 2019-09-30 16:33:06 PST

--
-- PostgreSQL database dump complete
--

\connect brem

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:06 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 4 (class 2615 OID 16393)
-- Name: problem1; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA problem1;


ALTER SCHEMA problem1 OWNER TO postgres;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2912 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 197 (class 1259 OID 16394)
-- Name: team; Type: TABLE; Schema: problem1; Owner: postgres
--

CREATE TABLE problem1.team (
    team_id integer NOT NULL,
    team_name character(20)
);


ALTER TABLE problem1.team OWNER TO postgres;

--
-- TOC entry 2904 (class 0 OID 16394)
-- Dependencies: 197
-- Data for Name: team; Type: TABLE DATA; Schema: problem1; Owner: postgres
--

COPY problem1.team (team_id, team_name) FROM stdin;
\.


-- Completed on 2019-09-30 16:33:07 PST

--
-- PostgreSQL database dump complete
--

\connect ima

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:07 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2916 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 197 (class 1259 OID 40963)
-- Name: employee; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.employee (
    emp_num numeric(6,0),
    emp_lname character varying(50) NOT NULL,
    emp_initial character varying(50),
    emp_fname character varying(50) NOT NULL,
    dept_code character varying(10) NOT NULL,
    job_code numeric(3,0)
);


ALTER TABLE public.employee OWNER TO postgres;

--
-- TOC entry 196 (class 1259 OID 32775)
-- Name: student; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.student (
    stu_num numeric(6,0),
    stu_lname character varying(50) NOT NULL,
    stu_fname character varying(50) NOT NULL,
    stu_init character varying(1),
    stu_dob date NOT NULL,
    stu_hrs integer NOT NULL,
    stu_class character varying(10) NOT NULL,
    stu_gpa numeric(3,2),
    stu_transfer character varying(3) NOT NULL,
    dept_code character varying(10) NOT NULL,
    stu_phone numeric(4,0),
    prof_num numeric(3,0)
);


ALTER TABLE public.student OWNER TO postgres;

--
-- TOC entry 2908 (class 0 OID 40963)
-- Dependencies: 197
-- Data for Name: employee; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.employee (emp_num, emp_lname, emp_initial, emp_fname, dept_code, job_code) FROM stdin;
11234	Friedman	k	Robert	MKTG	12
11238	Olanski	D	Delbert	MKTG	12
11241	Fontein		Juliette	INFS	5
11242	Cruazona	J	Maria	ENG	9
11245	Smithson	B	Bernard	INFS	6
11248	Washington	G	Oleta	ENGR	8
11256	McBride		Randall	ENGR	8
11257	Kachinn	D	Melanie	MKTG	14
11258	Smith	W	William	MKTG	14
11260	Ratula	A	Katrina	INFS	5
\.


--
-- TOC entry 2907 (class 0 OID 32775)
-- Dependencies: 196
-- Data for Name: student; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.student (stu_num, stu_lname, stu_fname, stu_init, stu_dob, stu_hrs, stu_class, stu_gpa, stu_transfer, dept_code, stu_phone, prof_num) FROM stdin;
321452	Bowser	William	C	1985-02-12	42	So	2.84	No	BIOL	2134	205
324257	Smithson	Anne	K	1991-11-15	81	Jr	3.27	Yes	CIS	2256	222
324258	Brewer	Julliete		1979-08-23	36	So	2.26	Yes	ACCT	2256	228
324269	Oblonski	Walter	H	1986-09-16	66	Jr	3.09	No	CIS	2114	222
324273	Smith	John	D	1968-12-30	102	Sr	2.11	Yes	ENGL	2231	199
324274	Katinga	Raphael	P	1989-10-21	114	Sr	3.15	No	ACCT	2267	228
324291	Robertson	Gerald	T	1983-04-08	120	Sr	3.87	No	EDU	2267	311
324299	Smith	John	B	1996-11-30	15	Fr	2.92	No	ACCT	2315	230
\.


-- Completed on 2019-09-30 16:33:08 PST

--
-- PostgreSQL database dump complete
--

\connect mydb

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:08 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 4 (class 2615 OID 16388)
-- Name: mydbschema; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA mydbschema;


ALTER SCHEMA mydbschema OWNER TO postgres;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2925 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 197 (class 1259 OID 16389)
-- Name: tabel1; Type: TABLE; Schema: mydbschema; Owner: postgres
--

CREATE TABLE mydbschema.tabel1 (
    id integer,
    password character(10)
);


ALTER TABLE mydbschema.tabel1 OWNER TO postgres;

--
-- TOC entry 199 (class 1259 OID 24619)
-- Name: store; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.store (
    store_id integer NOT NULL,
    store_name character varying(50) NOT NULL,
    store_location character varying(100) NOT NULL
);


ALTER TABLE public.store OWNER TO postgres;

--
-- TOC entry 198 (class 1259 OID 24617)
-- Name: store_store_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.store_store_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.store_store_id_seq OWNER TO postgres;

--
-- TOC entry 2926 (class 0 OID 0)
-- Dependencies: 198
-- Name: store_store_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.store_store_id_seq OWNED BY public.store.store_id;


--
-- TOC entry 2789 (class 2604 OID 24622)
-- Name: store store_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store ALTER COLUMN store_id SET DEFAULT nextval('public.store_store_id_seq'::regclass);


--
-- TOC entry 2915 (class 0 OID 16389)
-- Dependencies: 197
-- Data for Name: tabel1; Type: TABLE DATA; Schema: mydbschema; Owner: postgres
--

COPY mydbschema.tabel1 (id, password) FROM stdin;
\.


--
-- TOC entry 2917 (class 0 OID 24619)
-- Dependencies: 199
-- Data for Name: store; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.store (store_id, store_name, store_location) FROM stdin;
\.


--
-- TOC entry 2927 (class 0 OID 0)
-- Dependencies: 198
-- Name: store_store_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.store_store_id_seq', 1, false);


--
-- TOC entry 2791 (class 2606 OID 24624)
-- Name: store store_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store
    ADD CONSTRAINT store_pkey PRIMARY KEY (store_id);


--
-- TOC entry 2793 (class 2606 OID 24626)
-- Name: store store_store_name_key; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store
    ADD CONSTRAINT store_store_name_key UNIQUE (store_name);


-- Completed on 2019-09-30 16:33:09 PST

--
-- PostgreSQL database dump complete
--

\connect postgres

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:09 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 2932 (class 0 OID 0)
-- Dependencies: 2931
-- Name: DATABASE postgres; Type: COMMENT; Schema: -; Owner: postgres
--

COMMENT ON DATABASE postgres IS 'default administrative connection database';


--
-- TOC entry 8 (class 2615 OID 41091)
-- Name: group_1; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA group_1;


ALTER SCHEMA group_1 OWNER TO postgres;

--
-- TOC entry 4 (class 2615 OID 41127)
-- Name: roble_midterm; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA roble_midterm;


ALTER SCHEMA roble_midterm OWNER TO postgres;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2934 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 199 (class 1259 OID 41095)
-- Name: section; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.section (
    section_name character varying(50) NOT NULL,
    section_students character varying(50) NOT NULL
);


ALTER TABLE group_1.section OWNER TO postgres;

--
-- TOC entry 200 (class 1259 OID 41117)
-- Name: student_year_range; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.student_year_range (
    student_year_min integer NOT NULL,
    student_year_max integer NOT NULL,
    student_year_desc character varying(50) NOT NULL
);


ALTER TABLE group_1.student_year_range OWNER TO postgres;

--
-- TOC entry 198 (class 1259 OID 41092)
-- Name: students; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.students (
    student_name character varying(50) NOT NULL,
    student_course character varying(50) NOT NULL,
    student_year character varying(50) NOT NULL
);


ALTER TABLE group_1.students OWNER TO postgres;

--
-- TOC entry 202 (class 1259 OID 41131)
-- Name: professor; Type: TABLE; Schema: roble_midterm; Owner: postgres
--

CREATE TABLE roble_midterm.professor (
    prof_code integer,
    dept_code integer
);


ALTER TABLE roble_midterm.professor OWNER TO postgres;

--
-- TOC entry 201 (class 1259 OID 41128)
-- Name: student; Type: TABLE; Schema: roble_midterm; Owner: postgres
--

CREATE TABLE roble_midterm.student (
    stu_code integer,
    prof_code integer
);


ALTER TABLE roble_midterm.student OWNER TO postgres;

--
-- TOC entry 2922 (class 0 OID 41095)
-- Dependencies: 199
-- Data for Name: section; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.section (section_name, section_students) FROM stdin;
\.


--
-- TOC entry 2923 (class 0 OID 41117)
-- Dependencies: 200
-- Data for Name: student_year_range; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.student_year_range (student_year_min, student_year_max, student_year_desc) FROM stdin;
\.


--
-- TOC entry 2921 (class 0 OID 41092)
-- Dependencies: 198
-- Data for Name: students; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.students (student_name, student_course, student_year) FROM stdin;
S	Nacar	1st yr
\.


--
-- TOC entry 2925 (class 0 OID 41131)
-- Dependencies: 202
-- Data for Name: professor; Type: TABLE DATA; Schema: roble_midterm; Owner: postgres
--

COPY roble_midterm.professor (prof_code, dept_code) FROM stdin;
1	2
2	6
3	6
4	4
\.


--
-- TOC entry 2924 (class 0 OID 41128)
-- Dependencies: 201
-- Data for Name: student; Type: TABLE DATA; Schema: roble_midterm; Owner: postgres
--

COPY roble_midterm.student (stu_code, prof_code) FROM stdin;
100278	\N
128569	2
512272	4
531235	2
531235	\N
553427	1
\.


-- Completed on 2019-09-30 16:33:09 PST

--
-- PostgreSQL database dump complete
--

\connect store

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:09 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2943 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 199 (class 1259 OID 24655)
-- Name: employee; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.employee (
    employee_id integer NOT NULL,
    empolyee_firstname character varying(50),
    empolyee_lastname character varying(50),
    employee_hiredate date
);


ALTER TABLE public.employee OWNER TO postgres;

--
-- TOC entry 198 (class 1259 OID 24653)
-- Name: employee_employee_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.employee_employee_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.employee_employee_id_seq OWNER TO postgres;

--
-- TOC entry 2944 (class 0 OID 0)
-- Dependencies: 198
-- Name: employee_employee_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.employee_employee_id_seq OWNED BY public.employee.employee_id;


--
-- TOC entry 201 (class 1259 OID 24663)
-- Name: employs; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.employs (
    employs_id integer NOT NULL,
    store_id integer,
    employee_id integer
);


ALTER TABLE public.employs OWNER TO postgres;

--
-- TOC entry 200 (class 1259 OID 24661)
-- Name: employs_employs_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.employs_employs_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.employs_employs_id_seq OWNER TO postgres;

--
-- TOC entry 2945 (class 0 OID 0)
-- Dependencies: 200
-- Name: employs_employs_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.employs_employs_id_seq OWNED BY public.employs.employs_id;


--
-- TOC entry 197 (class 1259 OID 24645)
-- Name: store; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.store (
    store_id integer NOT NULL,
    store_name character varying(50) NOT NULL,
    store_location character varying(100) NOT NULL
);


ALTER TABLE public.store OWNER TO postgres;

--
-- TOC entry 196 (class 1259 OID 24643)
-- Name: store_store_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.store_store_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.store_store_id_seq OWNER TO postgres;

--
-- TOC entry 2946 (class 0 OID 0)
-- Dependencies: 196
-- Name: store_store_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.store_store_id_seq OWNED BY public.store.store_id;


--
-- TOC entry 2797 (class 2604 OID 24658)
-- Name: employee employee_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employee ALTER COLUMN employee_id SET DEFAULT nextval('public.employee_employee_id_seq'::regclass);


--
-- TOC entry 2798 (class 2604 OID 24666)
-- Name: employs employs_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employs ALTER COLUMN employs_id SET DEFAULT nextval('public.employs_employs_id_seq'::regclass);


--
-- TOC entry 2796 (class 2604 OID 24648)
-- Name: store store_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store ALTER COLUMN store_id SET DEFAULT nextval('public.store_store_id_seq'::regclass);


--
-- TOC entry 2933 (class 0 OID 24655)
-- Dependencies: 199
-- Data for Name: employee; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.employee (employee_id, empolyee_firstname, empolyee_lastname, employee_hiredate) FROM stdin;
\.


--
-- TOC entry 2935 (class 0 OID 24663)
-- Dependencies: 201
-- Data for Name: employs; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.employs (employs_id, store_id, employee_id) FROM stdin;
\.


--
-- TOC entry 2931 (class 0 OID 24645)
-- Dependencies: 197
-- Data for Name: store; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.store (store_id, store_name, store_location) FROM stdin;
\.


--
-- TOC entry 2947 (class 0 OID 0)
-- Dependencies: 198
-- Name: employee_employee_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.employee_employee_id_seq', 1, false);


--
-- TOC entry 2948 (class 0 OID 0)
-- Dependencies: 200
-- Name: employs_employs_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.employs_employs_id_seq', 1, false);


--
-- TOC entry 2949 (class 0 OID 0)
-- Dependencies: 196
-- Name: store_store_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.store_store_id_seq', 1, false);


--
-- TOC entry 2804 (class 2606 OID 24660)
-- Name: employee employee_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employee
    ADD CONSTRAINT employee_pkey PRIMARY KEY (employee_id);


--
-- TOC entry 2806 (class 2606 OID 24668)
-- Name: employs employs_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employs
    ADD CONSTRAINT employs_pkey PRIMARY KEY (employs_id);


--
-- TOC entry 2800 (class 2606 OID 24650)
-- Name: store store_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store
    ADD CONSTRAINT store_pkey PRIMARY KEY (store_id);


--
-- TOC entry 2802 (class 2606 OID 24652)
-- Name: store store_store_name_key; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.store
    ADD CONSTRAINT store_store_name_key UNIQUE (store_name);


--
-- TOC entry 2808 (class 2606 OID 24674)
-- Name: employs employs_employee_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employs
    ADD CONSTRAINT employs_employee_id_fkey FOREIGN KEY (employee_id) REFERENCES public.employee(employee_id);


--
-- TOC entry 2807 (class 2606 OID 24669)
-- Name: employs employs_store_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.employs
    ADD CONSTRAINT employs_store_id_fkey FOREIGN KEY (store_id) REFERENCES public.store(store_id);


-- Completed on 2019-09-30 16:33:10 PST

--
-- PostgreSQL database dump complete
--

\connect template1

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:10 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 2905 (class 0 OID 0)
-- Dependencies: 2904
-- Name: DATABASE template1; Type: COMMENT; Schema: -; Owner: postgres
--

COMMENT ON DATABASE template1 IS 'default template for new databases';


--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2907 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


-- Completed on 2019-09-30 16:33:10 PST

--
-- PostgreSQL database dump complete
--

\connect week10

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:10 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2972 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 203 (class 1259 OID 41027)
-- Name: barcelo_keyemployee; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_keyemployee (
    kemp_id integer NOT NULL,
    kemp_name character varying(25)
);


ALTER TABLE public.barcelo_keyemployee OWNER TO postgres;

--
-- TOC entry 202 (class 1259 OID 41025)
-- Name: barcelo_keyemployee_kemp_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.barcelo_keyemployee_kemp_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.barcelo_keyemployee_kemp_id_seq OWNER TO postgres;

--
-- TOC entry 2973 (class 0 OID 0)
-- Dependencies: 202
-- Name: barcelo_keyemployee_kemp_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.barcelo_keyemployee_kemp_id_seq OWNED BY public.barcelo_keyemployee.kemp_id;


--
-- TOC entry 207 (class 1259 OID 41044)
-- Name: barcelo_outcome; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_outcome (
    ship character varying(50) NOT NULL,
    battle character varying(50) NOT NULL,
    result character varying(50) NOT NULL
);


ALTER TABLE public.barcelo_outcome OWNER TO postgres;

--
-- TOC entry 196 (class 1259 OID 41003)
-- Name: barcelo_productnorth; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_productnorth (
    p_code numeric(6,0) NOT NULL,
    p_descript character varying(20) NOT NULL,
    price character varying(20) NOT NULL
);


ALTER TABLE public.barcelo_productnorth OWNER TO postgres;

--
-- TOC entry 197 (class 1259 OID 41008)
-- Name: barcelo_productsouth; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_productsouth (
    p_code numeric(6,0) NOT NULL,
    p_descript character varying(20) NOT NULL,
    price character varying(20) NOT NULL
);


ALTER TABLE public.barcelo_productsouth OWNER TO postgres;

--
-- TOC entry 198 (class 1259 OID 41013)
-- Name: barcelo_sales2019_quarter1; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_sales2019_quarter1 (
    s_agent character varying(20) NOT NULL,
    s_amount numeric(8,2) NOT NULL
);


ALTER TABLE public.barcelo_sales2019_quarter1 OWNER TO postgres;

--
-- TOC entry 199 (class 1259 OID 41016)
-- Name: barcelo_sales2019_quarter2; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_sales2019_quarter2 (
    s_agent character varying(20) NOT NULL,
    s_amount numeric(8,2) NOT NULL
);


ALTER TABLE public.barcelo_sales2019_quarter2 OWNER TO postgres;

--
-- TOC entry 206 (class 1259 OID 41041)
-- Name: barcelo_ship; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_ship (
    name character varying(50) NOT NULL,
    class character varying(50) NOT NULL,
    launched numeric(4,0) NOT NULL
);


ALTER TABLE public.barcelo_ship OWNER TO postgres;

--
-- TOC entry 200 (class 1259 OID 41019)
-- Name: barcelo_student; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_student (
    s_fname character varying(20),
    s_lname character varying(20)
);


ALTER TABLE public.barcelo_student OWNER TO postgres;

--
-- TOC entry 201 (class 1259 OID 41022)
-- Name: barcelo_studentassistant; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_studentassistant (
    s_fname character varying(20),
    s_lname character varying(20)
);


ALTER TABLE public.barcelo_studentassistant OWNER TO postgres;

--
-- TOC entry 205 (class 1259 OID 41035)
-- Name: barcelo_topemployee; Type: TABLE; Schema: public; Owner: postgres
--

CREATE TABLE public.barcelo_topemployee (
    temp_id integer NOT NULL,
    temp_name character varying(25)
);


ALTER TABLE public.barcelo_topemployee OWNER TO postgres;

--
-- TOC entry 204 (class 1259 OID 41033)
-- Name: barcelo_topemployee_temp_id_seq; Type: SEQUENCE; Schema: public; Owner: postgres
--

CREATE SEQUENCE public.barcelo_topemployee_temp_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.barcelo_topemployee_temp_id_seq OWNER TO postgres;

--
-- TOC entry 2974 (class 0 OID 0)
-- Dependencies: 204
-- Name: barcelo_topemployee_temp_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: postgres
--

ALTER SEQUENCE public.barcelo_topemployee_temp_id_seq OWNED BY public.barcelo_topemployee.temp_id;


--
-- TOC entry 2822 (class 2604 OID 41030)
-- Name: barcelo_keyemployee kemp_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_keyemployee ALTER COLUMN kemp_id SET DEFAULT nextval('public.barcelo_keyemployee_kemp_id_seq'::regclass);


--
-- TOC entry 2823 (class 2604 OID 41038)
-- Name: barcelo_topemployee temp_id; Type: DEFAULT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_topemployee ALTER COLUMN temp_id SET DEFAULT nextval('public.barcelo_topemployee_temp_id_seq'::regclass);


--
-- TOC entry 2960 (class 0 OID 41027)
-- Dependencies: 203
-- Data for Name: barcelo_keyemployee; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_keyemployee (kemp_id, kemp_name) FROM stdin;
165232	Joyce Edwards
835438	Diane Collins
284322	Heather Morris
332444	Doris Reed
\.


--
-- TOC entry 2964 (class 0 OID 41044)
-- Dependencies: 207
-- Data for Name: barcelo_outcome; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_outcome (ship, battle, result) FROM stdin;
Bismarck	North Atlantic	sunk
California	Guadalcanal	damaged
California	Surigao Strait	OK
Duke of York	North Cape	OK
Fuso	Surigao Strait	sunk
Hood	North Atlantic	sunk
King George V	North Atlantic	OK
Kirishima	Guadalcanal	sunk
Prince of Wales	North Atlantic	damaged
Rodney	North Atlantic	OK
Schamhorst	North Cape	sunk
South Dakota	Guadalcanal	damaged
Tennessee	Surigao Strait	OK
Washington	Guadalcanal	OK
West Virginia	Surigao Strait	OK
Yamashiro	Surigao Strait	sunk
\.


--
-- TOC entry 2953 (class 0 OID 41003)
-- Dependencies: 196
-- Data for Name: barcelo_productnorth; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_productnorth (p_code, p_descript, price) FROM stdin;
123456	Flasghlight	5.26
123457	lamp	25.15
123458	Box fan	10.99
213345	9v Battery	1.92
254467	100W bulb	1.47
311452	powerdrill	34.99
\.


--
-- TOC entry 2954 (class 0 OID 41008)
-- Dependencies: 197
-- Data for Name: barcelo_productsouth; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_productsouth (p_code, p_descript, price) FROM stdin;
345679	Dishwasher	500.00
123458	Box fan	10.99
345678	Microwave	160.00
\.


--
-- TOC entry 2955 (class 0 OID 41013)
-- Dependencies: 198
-- Data for Name: barcelo_sales2019_quarter1; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_sales2019_quarter1 (s_agent, s_amount) FROM stdin;
Mike	150000.25
Jon	132000.75
Mary	100000.00
\.


--
-- TOC entry 2956 (class 0 OID 41016)
-- Dependencies: 199
-- Data for Name: barcelo_sales2019_quarter2; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_sales2019_quarter2 (s_agent, s_amount) FROM stdin;
Mike	120000.25
Jon	142000.75
Mary	100000.00
\.


--
-- TOC entry 2963 (class 0 OID 41041)
-- Dependencies: 206
-- Data for Name: barcelo_ship; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_ship (name, class, launched) FROM stdin;
California	Tennessee	1921
Haruna	Kongo	1916
Hiei	Kongo	1914
Iowa	Iowa	1943
Kirishima	Kongo	1915
Kongo	Kongo	1913
Missouri	Iowa	1944
Musashi	Yamato	1942
New Jersey	Iowa	1943
North Carolina	North Carolina	1941
Ramillies	Revenge	1917
Renown	Renown	1916
Repulse	Renown	1916
Resolution	Renown	1916
Revenge	Revenge	1916
Royal Oak	Revenge	1916
Royal Sovereign	Revenge	1916
South Dakota	North Carolina	1941
Tennessee	Tennessee	1920
Washington	North Carolina	1941
Wisconsin	Iowa	1944
Yamato	Yamato	1941
\.


--
-- TOC entry 2957 (class 0 OID 41019)
-- Dependencies: 200
-- Data for Name: barcelo_student; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_student (s_fname, s_lname) FROM stdin;
George	Jones
Jane	Smith
Peter	Robinson
Franklin	Johnson
Martin	Lopez
\.


--
-- TOC entry 2958 (class 0 OID 41022)
-- Dependencies: 201
-- Data for Name: barcelo_studentassistant; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_studentassistant (s_fname, s_lname) FROM stdin;
Franklin	Lopez
William	Turner
Franklin	Johnson
Susan	Rogers
\.


--
-- TOC entry 2962 (class 0 OID 41035)
-- Dependencies: 205
-- Data for Name: barcelo_topemployee; Type: TABLE DATA; Schema: public; Owner: postgres
--

COPY public.barcelo_topemployee (temp_id, temp_name) FROM stdin;
677655	Evelyn Morgan
835438	Diane Collins
284322	Heather Morris
345334	Jean Bell
\.


--
-- TOC entry 2975 (class 0 OID 0)
-- Dependencies: 202
-- Name: barcelo_keyemployee_kemp_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.barcelo_keyemployee_kemp_id_seq', 1, false);


--
-- TOC entry 2976 (class 0 OID 0)
-- Dependencies: 204
-- Name: barcelo_topemployee_temp_id_seq; Type: SEQUENCE SET; Schema: public; Owner: postgres
--

SELECT pg_catalog.setval('public.barcelo_topemployee_temp_id_seq', 1, false);


--
-- TOC entry 2829 (class 2606 OID 41032)
-- Name: barcelo_keyemployee barcelo_keyemployee_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_keyemployee
    ADD CONSTRAINT barcelo_keyemployee_pkey PRIMARY KEY (kemp_id);


--
-- TOC entry 2825 (class 2606 OID 41007)
-- Name: barcelo_productnorth barcelo_productnorth_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_productnorth
    ADD CONSTRAINT barcelo_productnorth_pkey PRIMARY KEY (p_code);


--
-- TOC entry 2827 (class 2606 OID 41012)
-- Name: barcelo_productsouth barcelo_productsouth_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_productsouth
    ADD CONSTRAINT barcelo_productsouth_pkey PRIMARY KEY (p_code);


--
-- TOC entry 2831 (class 2606 OID 41040)
-- Name: barcelo_topemployee barcelo_topemployee_pkey; Type: CONSTRAINT; Schema: public; Owner: postgres
--

ALTER TABLE ONLY public.barcelo_topemployee
    ADD CONSTRAINT barcelo_topemployee_pkey PRIMARY KEY (temp_id);


-- Completed on 2019-09-30 16:33:11 PST

--
-- PostgreSQL database dump complete
--

\connect workgroup

SET default_transaction_read_only = off;

--
-- PostgreSQL database dump
--

-- Dumped from database version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)
-- Dumped by pg_dump version 10.10 (Ubuntu 10.10-0ubuntu0.18.04.1)

-- Started on 2019-09-30 16:33:11 PST

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- TOC entry 8 (class 2615 OID 41098)
-- Name: group_1; Type: SCHEMA; Schema: -; Owner: postgres
--

CREATE SCHEMA group_1;


ALTER SCHEMA group_1 OWNER TO postgres;

--
-- TOC entry 1 (class 3079 OID 13039)
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- TOC entry 2927 (class 0 OID 0)
-- Dependencies: 1
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- TOC entry 198 (class 1259 OID 41114)
-- Name: section; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.section (
    section_id character varying(50) NOT NULL,
    section_name character varying(50) NOT NULL,
    section_students character varying(50) NOT NULL,
    section_year character varying(50) NOT NULL
);


ALTER TABLE group_1.section OWNER TO postgres;

--
-- TOC entry 200 (class 1259 OID 41123)
-- Name: student; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.student (
    student_year integer NOT NULL,
    student_name character varying(50) NOT NULL
);


ALTER TABLE group_1.student OWNER TO postgres;

--
-- TOC entry 199 (class 1259 OID 41120)
-- Name: student_year_range; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.student_year_range (
    student_year_min integer NOT NULL,
    student_year_max integer NOT NULL,
    student_year_desc character varying(50) NOT NULL
);


ALTER TABLE group_1.student_year_range OWNER TO postgres;

--
-- TOC entry 197 (class 1259 OID 41111)
-- Name: students; Type: TABLE; Schema: group_1; Owner: postgres
--

CREATE TABLE group_1.students (
    student_id character varying(50) NOT NULL,
    student_name character varying(50) NOT NULL,
    student_course character varying(50) NOT NULL,
    student_year character varying(50) NOT NULL,
    section_id character varying(50) NOT NULL
);


ALTER TABLE group_1.students OWNER TO postgres;

--
-- TOC entry 2917 (class 0 OID 41114)
-- Dependencies: 198
-- Data for Name: section; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.section (section_id, section_name, section_students, section_year) FROM stdin;
10	A	Asma	2nd yr
11	B	Barcelo	2nd yr
12	C	Miras	2nd yr
13	D	Pio	2nd yr
14	E	Surigao	2nd yr
15	F	Perez	1st yr
16	G	Pia	1st yr
\.


--
-- TOC entry 2919 (class 0 OID 41123)
-- Dependencies: 200
-- Data for Name: student; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.student (student_year, student_name) FROM stdin;
1	Asma
2	Barcelo
3	Pio
4	Surigao
\.


--
-- TOC entry 2918 (class 0 OID 41120)
-- Dependencies: 199
-- Data for Name: student_year_range; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.student_year_range (student_year_min, student_year_max, student_year_desc) FROM stdin;
1	2	Young 1st or 2nd
3	4	Old 3rd or 4th
\.


--
-- TOC entry 2916 (class 0 OID 41111)
-- Dependencies: 197
-- Data for Name: students; Type: TABLE DATA; Schema: group_1; Owner: postgres
--

COPY group_1.students (student_id, student_name, student_course, student_year, section_id) FROM stdin;
1	Asma	BSIT	2nd yr	10
2	Barcelo	BSMT	2nd yr	11
3	Miras	TM	2nd yr	12
4	Pio	HRM	2nd yr	13
5	Surigao	Pharma	2nd yr	14
6	Perez	MLS	1st yr	15
7	Pia	MLS	1st yr	16
\.


-- Completed on 2019-09-30 16:33:12 PST

--
-- PostgreSQL database dump complete
--

-- Completed on 2019-09-30 16:33:12 PST

--
-- PostgreSQL database cluster dump complete
--
