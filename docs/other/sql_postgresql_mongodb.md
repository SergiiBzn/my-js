<a name="top"></a>

[На главную](../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | SQL |
|1 | [Was ist SQL und wofür wird es verwendet?](#1) |
|2 | [Unterschied zwischen SQL und NoSQL?](#2) |
|3 | [Was ist ein Primärschlüssel?](#3) |
|4 | [Was ist ein Fremdschlüssel?](#4) |
|5 | [Unterschied zwischen PRIMARY KEY, UNIQUE und INDEX?](#5) |
|6 | [Was sind Normalformen und warum sind sie wichtig?](#6) |
|7 | [Unterschied zwischen 1NF, 2NF und 3NF?](#7) |
|8 | [Was sind Transaktionen in SQL?](#8) |
|9 | [Was bedeutet ACID in Datenbanken?](#9) |
|10 | [Unterschied zwischen ACID und BASE Prinzipien?](#10) |
|11 | [Unterschied zwischen SELECT * und gezielten Spaltenabfragen?](#11) |
|12 | [Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN?](#12) |
|13 | [Unterschied zwischen WHERE und HAVING?](#13) |
|14 | [Unterschied zwischen DISTINCT und GROUP BY?](#14) |
|15 | [Was sind Aggregatfunktionen (COUNT, SUM, AVG, MIN, MAX)?](#15) |
|16 | [Wie funktioniert ORDER BY und LIMIT?](#16) |
|17 | [Was ist ein Subquery (Unterabfrage)?](#17) |
|18 | [Unterschied zwischen korrelierter und nicht-korrelierter Unterabfrage?](#18) |
|19 | [Unterschied zwischen EXISTS und IN?](#19) |
|20 | [Unterschied zwischen UNION und UNION ALL?](#20) |
|   | PostgreSQL |
|21 | [Was ist PostgreSQL und welche Vorteile hat es gegenüber MySQL?](#21) |
|22 | [Was sind Datentypen in PostgreSQL (TEXT, VARCHAR, SERIAL, JSONB)?](#22) |
|23 | [Unterschied zwischen SERIAL und BIGSERIAL?](#23) |
|24 | [Wie arbeitet PostgreSQL mit Arrays?](#24) |
|25 | [Was ist der Unterschied zwischen JSON und JSONB in PostgreSQL?](#25) |
|26 | [Wie speichert und verarbeitet PostgreSQL Zeitstempel (TIMESTAMP, TIMESTAMPTZ)?](#26) |
|27 | [Was sind Sequences in PostgreSQL?](#27) |
|28 | [Wie implementiert man Auto-Increment in PostgreSQL?](#28) |
|29 | [Was sind Materialized Views?](#29) |
|30 | [Unterschied zwischen View und Materialized View?](#30) |
|31 | [Was ist ein Index in PostgreSQL?](#31) |
|32 | [Unterschied zwischen B-Tree, Hash und GIN Index?](#32) |
|33 | [Was ist ein Unique Index?](#33) |
|34 | [Nachteile von zu vielen Indexen?](#34) |
|35 | [Wie analysiert man eine Query mit EXPLAIN?](#35) |
|36 | [Unterschied zwischen EXPLAIN und EXPLAIN ANALYZE?](#36) |
|37 | [Wie vermeidet man Table Scans?](#37) |
|38 | [Was ist ein Partial Index?](#38) |
|39 | [Was ist ein Covering Index (INCLUDE)?](#39) |
|40 | [Wie funktioniert Vacuum in PostgreSQL?](#40) |
|41 | [Wie startet und beendet man eine Transaktion?](#41) |
|42 | [Unterschied zwischen COMMIT und ROLLBACK?](#42) |
|43 | [Was ist ein Savepoint in SQL?](#43) |
|44 | [Unterschied zwischen Deadlock und Race Condition?](#44) |
|45 | [Welche Isolation Levels gibt es in PostgreSQL (READ COMMITTED, SERIALIZABLE)?](#45) |
|46 | [Unterschied zwischen Optimistic Locking und Pessimistic Locking?](#46) |
|47 | [Wie erkennt PostgreSQL Deadlocks?](#47) |
|48 | [Welche Standard-Isolationsebene nutzt PostgreSQL?](#48) |
|49 | [Wie implementiert man Transaktionen in Node.js/Express mit PostgreSQL?](#49) |
|50 | [Unterschied zwischen BEGIN und START TRANSACTION?](#50) |
|51 | [Wie verwaltet man Benutzer und Rollen in PostgreSQL?](#51) |
|52 | [Unterschied zwischen Login-Rollen und Gruppen-Rollen?](#52) |
|53 | [Wie vergibt man Berechtigungen (GRANT, REVOKE)?](#53) |
|54 | [Was ist Row Level Security (RLS) in PostgreSQL?](#54) |
|55 | [Wie schützt man sensible Daten (z. B. Passwörter) in PostgreSQL?](#55) |
|56 | [Wie sichert man eine PostgreSQL-Datenbank (pg_dump)?](#56) |
|57 | [Wie stellt man ein Backup wieder her?](#57) |
|58 | [Unterschied zwischen pg_dump und pg_restore?](#58) |
|59 | [Wie konfiguriert man SSL für PostgreSQL-Verbindungen?](#59) |
|60 | [Was ist Connection Pooling und wie implementiert man es (z. B. mit pg-pool in Node.js)?](#60) |
|   | MongoDB |
|61 | [Was ist MongoDB und wofür wird es verwendet?](#61) |
|62 | [Unterschied zwischen SQL und NoSQL?](#62) |
|63 | [Was ist der Unterschied zwischen Dokument, Collection und Datenbank?](#63) |
|64 | [Was ist BSON und wie unterscheidet es sich von JSON?](#64) |
|65 | [Was ist ein ObjectId und warum wird es genutzt?](#65) |
|66 | [Wie fügt man Dokumente ein (insertOne, insertMany)?](#66) |
|67 | [Wie liest man Daten (find, findOne)?](#67) |
|68 | [Unterschied zwischen find(), findOne() und findById() in Mongoose?](#68) |
|69 | [Wie aktualisiert man Dokumente (updateOne, updateMany, findByIdAndUpdate)?](#69) |
|70 | [Wie löscht man Dokumente (deleteOne, deleteMany, findByIdAndDelete)?](#70) |
|71 | [Was ist Mongoose und warum wird es häufig in Node/Express-Projekten verwendet?](#71) |
|72 | [Unterschied zwischen Schema und Model in Mongoose?](#72) |
|73 | [Wie definiert man Validierungen in einem Schema?](#73) |
|74 | [Was sind Virtuals und Middleware (pre, post) in Mongoose?](#74) |
|75 | [Wie funktioniert populate in Mongoose (Beziehungen zwischen Dokumenten)?](#75) |
|76 | [Welche Vergleichsoperatoren gibt es ($gt, $lt, $in, $nin, $eq)?](#76) |
|77 | [Wie sucht man mit $and, $or, $nor?](#77) |
|78 | [Wie sucht man in Arrays ($elemMatch, $push, $pull)?](#78) |
|79 | [Unterschied zwischen sort, limit und skip?](#79) |
|80 | [Was ist der Unterschied zwischen countDocuments() und estimatedDocumentCount()?](#80) |
|81 | [Was ist eine Aggregation Pipeline und wofür wird sie verwendet?](#81) |
|82 | [Welche Stages gibt es ($match, $group, $project, $sort, $limit)?](#82) |
|83 | [Was sind Indexe und warum sind sie wichtig?](#83) |
|84 | [Unterschied zwischen Single-Field Index und Compound Index?](#84) |
|85 | [Was ist ein Unique-Index?](#85) |
|86 | [Was ist Sharding und Replikation in MongoDB?](#86) |
|87 | [Was ist ein Replica Set und warum ist es wichtig?](#87) |
|88 | [Wie optimiert man Queries in MongoDB (Explain, Indexe)?](#88) |
|89 | [Wie schützt man MongoDB vor unautorisiertem Zugriff?](#89) |
|90 | [Unterschied zwischen Rollen und Berechtigungen (z. B. read, readWrite)?](#90) |
|91 | [](#91) |
|92 | [](#92) |
|93 | [](#93) |
|94 | [](#94) |
|95 | [](#95) |
|96 | [](#96) |
|97 | [](#97) |
|98 | [](#98) |
|99 | [](#99) |
|100 | [](#100) |
|101 | [](#101) |
|102 | [](#102) |
|103 | [](#103) |
|104 | [](#104) |
|105 | [](#105) |
|106 | [](#106) |
|107 | [](#107) |
|108 | [](#108) |
|109 | [](#109) |
|110 | [](#110) |
|111 | [](#111) |
|112 | [](#112) |
|113 | [](#113) |
|114 | [](#114) |
|115 | [](#115) |
|116 | [](#116) |
|117 | [](#117) |
|118 | [](#118) |
|119 | [](#119) |
|120 | [](#120) |
|121 | [](#121) |
|122 | [](#122) |
|123 | [](#123) |
|124 | [](#124) |
|125 | [](#125) |
|126 | [](#126) |
|127 | [](#127) |
|128 | [](#128) |
|129 | [](#129) |
|130 | [](#130) |
|131 | [](#131) |
|132 | [](#132) |
|133 | [](#133) |
|134 | [](#134) |
|135 | [](#135) |
|136 | [](#136) |
|137 | [](#137) |
|138 | [](#138) |
|139 | [](#139) |
|140 | [](#140) |
|141 | [](#141) |
|142 | [](#142) |
|143 | [](#143) |
|144 | [](#144) |
|145 | [](#145) |
|146 | [](#146) |
|147 | [](#147) |
|148 | [](#148) |
|149 | [](#149) |
|150 | [](#150) |
|151 | [](#151) |
|152 | [](#152) |
|153 | [](#153) |
|154 | [](#154) |
|155 | [](#155) |
|156 | [](#156) |
|157 | [](#157) |
|158 | [](#158) |
|159 | [](#159) |
|160 | [](#160) |
|161 | [](#161) |
|162 | [](#162) |
|163 | [](#163) |
|164 | [](#164) |
|165 | [](#165) |
|166 | [](#166) |
|167 | [](#167) |
|168 | [](#168) |
|169 | [](#169) |
|170 | [](#170) |
|171 | [](#171) |
|172 | [](#172) |
|173 | [](#173) |
|174 | [](#174) |
|175 | [](#175) |
|176 | [](#176) |
|177 | [](#177) |
|178 | [](#178) |
|179 | [](#179) |
|180 | [](#180) |
|181 | [](#181) |
|182 | [](#182) |
|183 | [](#183) |
|184 | [](#184) |
|185 | [](#185) |
|186 | [](#186) |
|187 | [](#187) |
|188 | [](#188) |
|189 | [](#189) |
|190 | [](#190) |
|191 | [](#191) |
|192 | [](#192) |
|193 | [](#193) |
|194 | [](#194) |
|195 | [](#195) |
|196 | [](#196) |
|197 | [](#197) |
|198 | [](#198) |
|199 | [](#199) |
|200 | [](#200) |



<a name="questions"></a>


  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> 



  **[⬆ Наверх](#top)**

2. ### <a name="2"></a> 



  **[⬆ Наверх](#top)**

3. ### <a name="3"></a> 



  **[⬆ Наверх](#top)**

4. ### <a name="4"></a> 



  **[⬆ Наверх](#top)**

5. ### <a name="5"></a> 



  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> 



  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> 



  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> 



  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> 



  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> 



  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> 



  **[⬆ Наверх](#top)**

12. ### <a name="12"></a> 



  **[⬆ Наверх](#top)**

13. ### <a name="13"></a> 



  **[⬆ Наверх](#top)**

14. ### <a name="14"></a> 



  **[⬆ Наверх](#top)**

15. ### <a name="15"></a> 



  **[⬆ Наверх](#top)**

16. ### <a name="16"></a> 



  **[⬆ Наверх](#top)**

17. ### <a name="17"></a> 



  **[⬆ Наверх](#top)**

18. ### <a name="18"></a> 



  **[⬆ Наверх](#top)**

19. ### <a name="19"></a> 



  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> 



  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> 



  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> 



  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> 



  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> 



  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> 



  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> 



  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> 



  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> 



  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> 



  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> 



  **[⬆ Наверх](#top)**  

31. ### <a name="31"></a> 



  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> 



  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> 



  **[⬆ Наверх](#top)**

34. ### <a name="34"></a> 



  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> 



  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> 



  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> 



  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> 



  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> 



  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> 



  **[⬆ Наверх](#top)**  

41. ### <a name="41"></a> 



  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> 



  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> 



  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> 



  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> 



  **[⬆ Наверх](#top)**

46. ### <a name="46"></a> 



  **[⬆ Наверх](#top)**

47. ### <a name="47"></a> 



  **[⬆ Наверх](#top)**

48. ### <a name="48"></a> 



  **[⬆ Наверх](#top)**

49. ### <a name="49"></a> 



  **[⬆ Наверх](#top)**

50. ### <a name="50"></a> 



  **[⬆ Наверх](#top)**  

51. ### <a name="51"></a> 



  **[⬆ Наверх](#top)**

52. ### <a name="52"></a> 



  **[⬆ Наверх](#top)**

53. ### <a name="53"></a> 



  **[⬆ Наверх](#top)**

54. ### <a name="54"></a> 



  **[⬆ Наверх](#top)**

55. ### <a name="55"></a> 



  **[⬆ Наверх](#top)**

56. ### <a name="56"></a> 



  **[⬆ Наверх](#top)**

57. ### <a name="57"></a> 



  **[⬆ Наверх](#top)**

58. ### <a name="58"></a> 



  **[⬆ Наверх](#top)**

59. ### <a name="59"></a> 



  **[⬆ Наверх](#top)**

60. ### <a name="60"></a> 



  **[⬆ Наверх](#top)**

61. ### <a name="61"></a> 



  **[⬆ Наверх](#top)**

62. ### <a name="62"></a> 



  **[⬆ Наверх](#top)**

63. ### <a name="63"></a> 



  **[⬆ Наверх](#top)**

64. ### <a name="64"></a> 



  **[⬆ Наверх](#top)**

65. ### <a name="65"></a> 



  **[⬆ Наверх](#top)**

66. ### <a name="66"></a> 



  **[⬆ Наверх](#top)**

67. ### <a name="67"></a> 



  **[⬆ Наверх](#top)**

68. ### <a name="68"></a> 



  **[⬆ Наверх](#top)**

69. ### <a name="69"></a> 



  **[⬆ Наверх](#top)**

70. ### <a name="70"></a> 



  **[⬆ Наверх](#top)**

71. ### <a name="71"></a> 



  **[⬆ Наверх](#top)**

72. ### <a name="72"></a> 



  **[⬆ Наверх](#top)**

73. ### <a name="73"></a> 



  **[⬆ Наверх](#top)**

74. ### <a name="74"></a> 



  **[⬆ Наверх](#top)**

75. ### <a name="75"></a> 



  **[⬆ Наверх](#top)**

76. ### <a name="76"></a> 



  **[⬆ Наверх](#top)**

77. ### <a name="77"></a> 



  **[⬆ Наверх](#top)**

78. ### <a name="78"></a> 



  **[⬆ Наверх](#top)**

79. ### <a name="79"></a> 



  **[⬆ Наверх](#top)**

80. ### <a name="80"></a> 



  **[⬆ Наверх](#top)**  

81. ### <a name="81"></a> 



  **[⬆ Наверх](#top)**

82. ### <a name="82"></a> 



  **[⬆ Наверх](#top)**

83. ### <a name="83"></a> 



  **[⬆ Наверх](#top)**

84. ### <a name="84"></a> 



  **[⬆ Наверх](#top)**

85. ### <a name="85"></a> 



  **[⬆ Наверх](#top)**

86. ### <a name="86"></a> 



  **[⬆ Наверх](#top)**

87. ### <a name="87"></a> 



  **[⬆ Наверх](#top)**

88. ### <a name="88"></a> 



  **[⬆ Наверх](#top)**

89. ### <a name="89"></a> 



  **[⬆ Наверх](#top)**

90. ### <a name="90"></a> 



  **[⬆ Наверх](#top)**  

91. ### <a name="91"></a> 



  **[⬆ Наверх](#top)**

92. ### <a name="92"></a> 



  **[⬆ Наверх](#top)**

93. ### <a name="93"></a> 



  **[⬆ Наверх](#top)**

94. ### <a name="94"></a> 



  **[⬆ Наверх](#top)**

95. ### <a name="95"></a> 



  **[⬆ Наверх](#top)**

96. ### <a name="96"></a> 



  **[⬆ Наверх](#top)**

97. ### <a name="97"></a> 



  **[⬆ Наверх](#top)**

98. ### <a name="98"></a> 



  **[⬆ Наверх](#top)**

99. ### <a name="99"></a> 



  **[⬆ Наверх](#top)**

100. ### <a name="100"></a> 



  **[⬆ Наверх](#top)**    

101. ### <a name="101"></a> 



  **[⬆ Наверх](#top)**

102. ### <a name="102"></a> 



  **[⬆ Наверх](#top)**

103. ### <a name="103"></a> 



  **[⬆ Наверх](#top)**

104. ### <a name="104"></a> 



  **[⬆ Наверх](#top)**

105. ### <a name="105"></a> 



  **[⬆ Наверх](#top)**

106. ### <a name="106"></a> 



  **[⬆ Наверх](#top)**

107. ### <a name="107"></a> 



  **[⬆ Наверх](#top)**

108. ### <a name="108"></a> 



  **[⬆ Наверх](#top)**

109. ### <a name="109"></a> 



  **[⬆ Наверх](#top)**

110. ### <a name="110"></a> 



  **[⬆ Наверх](#top)**

111. ### <a name="111"></a> 



  **[⬆ Наверх](#top)**

112. ### <a name="112"></a> 



  **[⬆ Наверх](#top)**

113. ### <a name="113"></a> 



  **[⬆ Наверх](#top)**

114. ### <a name="114"></a> 



  **[⬆ Наверх](#top)**

115. ### <a name="115"></a> 



  **[⬆ Наверх](#top)**

116. ### <a name="116"></a> 



  **[⬆ Наверх](#top)**

117. ### <a name="117"></a> 



  **[⬆ Наверх](#top)**

118. ### <a name="118"></a> 



  **[⬆ Наверх](#top)**

119. ### <a name="119"></a> 



  **[⬆ Наверх](#top)**

120. ### <a name="120"></a> 



  **[⬆ Наверх](#top)**

121. ### <a name="121"></a> 



  **[⬆ Наверх](#top)**

122. ### <a name="122"></a> 



  **[⬆ Наверх](#top)**

123. ### <a name="123"></a> 



  **[⬆ Наверх](#top)**

124. ### <a name="124"></a> 



  **[⬆ Наверх](#top)**

125. ### <a name="125"></a> 



  **[⬆ Наверх](#top)**

126. ### <a name="126"></a> 



  **[⬆ Наверх](#top)**

127. ### <a name="127"></a> 



  **[⬆ Наверх](#top)**

128. ### <a name="128"></a> 



  **[⬆ Наверх](#top)**

129. ### <a name="129"></a> 



  **[⬆ Наверх](#top)**

130. ### <a name="130"></a> 



  **[⬆ Наверх](#top)**  

131. ### <a name="131"></a> 



  **[⬆ Наверх](#top)**

132. ### <a name="132"></a> 



  **[⬆ Наверх](#top)**

133. ### <a name="133"></a> 



  **[⬆ Наверх](#top)**

134. ### <a name="134"></a> 



  **[⬆ Наверх](#top)**

135. ### <a name="135"></a> 



  **[⬆ Наверх](#top)**

136. ### <a name="136"></a> 



  **[⬆ Наверх](#top)**

137. ### <a name="137"></a> 



  **[⬆ Наверх](#top)**

138. ### <a name="138"></a> 



  **[⬆ Наверх](#top)**

139. ### <a name="139"></a> 



  **[⬆ Наверх](#top)**

140. ### <a name="140"></a> 



  **[⬆ Наверх](#top)**  

141. ### <a name="141"></a> 



  **[⬆ Наверх](#top)**

142. ### <a name="142"></a> 



  **[⬆ Наверх](#top)**

143. ### <a name="143"></a> 



  **[⬆ Наверх](#top)**

144. ### <a name="144"></a> 



  **[⬆ Наверх](#top)**

145. ### <a name="145"></a> 



  **[⬆ Наверх](#top)**

146. ### <a name="146"></a> 



  **[⬆ Наверх](#top)**

147. ### <a name="147"></a> 



  **[⬆ Наверх](#top)**

148. ### <a name="148"></a> 



  **[⬆ Наверх](#top)**

149. ### <a name="149"></a> 



  **[⬆ Наверх](#top)**

150. ### <a name="150"></a> 



  **[⬆ Наверх](#top)**  

151. ### <a name="151"></a> 



  **[⬆ Наверх](#top)**

152. ### <a name="152"></a> 



  **[⬆ Наверх](#top)**

153. ### <a name="153"></a> 



  **[⬆ Наверх](#top)**

154. ### <a name="154"></a> 



  **[⬆ Наверх](#top)**

155. ### <a name="155"></a> 



  **[⬆ Наверх](#top)**

156. ### <a name="156"></a> 



  **[⬆ Наверх](#top)**

157. ### <a name="157"></a> 



  **[⬆ Наверх](#top)**

158. ### <a name="158"></a> 



  **[⬆ Наверх](#top)**

159. ### <a name="159"></a> 



  **[⬆ Наверх](#top)**

160. ### <a name="160"></a> 



  **[⬆ Наверх](#top)**

161. ### <a name="161"></a> 



  **[⬆ Наверх](#top)**

162. ### <a name="162"></a> 



  **[⬆ Наверх](#top)**

163. ### <a name="163"></a> 



  **[⬆ Наверх](#top)**

164. ### <a name="164"></a> 



  **[⬆ Наверх](#top)**

165. ### <a name="165"></a> 



  **[⬆ Наверх](#top)**

166. ### <a name="166"></a> 



  **[⬆ Наверх](#top)**

167. ### <a name="167"></a> 



  **[⬆ Наверх](#top)**

168. ### <a name="168"></a> 



  **[⬆ Наверх](#top)**

169. ### <a name="169"></a> 



  **[⬆ Наверх](#top)**

170. ### <a name="170"></a> 



  **[⬆ Наверх](#top)**

171. ### <a name="171"></a> 



  **[⬆ Наверх](#top)**

172. ### <a name="172"></a> 



  **[⬆ Наверх](#top)**

173. ### <a name="173"></a> 



  **[⬆ Наверх](#top)**

174. ### <a name="174"></a> 



  **[⬆ Наверх](#top)**

175. ### <a name="175"></a> 



  **[⬆ Наверх](#top)**

176. ### <a name="176"></a> 



  **[⬆ Наверх](#top)**

177. ### <a name="177"></a> 



  **[⬆ Наверх](#top)**

178. ### <a name="178"></a> 



  **[⬆ Наверх](#top)**

179. ### <a name="179"></a> 



  **[⬆ Наверх](#top)**

180. ### <a name="180"></a> 



  **[⬆ Наверх](#top)**  

181. ### <a name="181"></a> 



  **[⬆ Наверх](#top)**

182. ### <a name="182"></a> 



  **[⬆ Наверх](#top)**

183. ### <a name="183"></a> 



  **[⬆ Наверх](#top)**

184. ### <a name="184"></a> 



  **[⬆ Наверх](#top)**

185. ### <a name="185"></a> 



  **[⬆ Наверх](#top)**

186. ### <a name="186"></a> 



  **[⬆ Наверх](#top)**

187. ### <a name="187"></a> 



  **[⬆ Наверх](#top)**

188. ### <a name="188"></a> 



  **[⬆ Наверх](#top)**

189. ### <a name="189"></a> 



  **[⬆ Наверх](#top)**

190. ### <a name="190"></a> 



  **[⬆ Наверх](#top)**  

191. ### <a name="191"></a> 



  **[⬆ Наверх](#top)**

192. ### <a name="192"></a> 



  **[⬆ Наверх](#top)**

193. ### <a name="193"></a> 



  **[⬆ Наверх](#top)**

194. ### <a name="194"></a> 



  **[⬆ Наверх](#top)**

195. ### <a name="195"></a> 



  **[⬆ Наверх](#top)**

196. ### <a name="196"></a> 



  **[⬆ Наверх](#top)**

197. ### <a name="197"></a> 



  **[⬆ Наверх](#top)**

198. ### <a name="198"></a> 



  **[⬆ Наверх](#top)**

199. ### <a name="199"></a> 



  **[⬆ Наверх](#top)**

200. ### <a name="200"></a> 



  **[⬆ Наверх](#top)**      
