% Fatos
atomo(p).
atomo(q).
atomo(r).
atomo(s).
atomo(t).
atomo(u).
atomo(v).
negacao(~).
atomo(negacao,p).
atomo(negacao,q).
atomo(negacao,r).
atomo(negacao,s).
atomo(negacao,t).
atomo(negacao,u).
atomo(negacao,v).
conectivo(&).
conectivo(#).
conectivo(>).
auxiliar1(/).
auxiliar2(\).

formula(X,Y):- negacao(X),atomo(Y). % % exemplo teste: formula(~,p).
formula(X,Y,Z) :- atomo(X),conectivo(Y),atomo(Z) . % exemplo teste: formula(p,>,q,).
formula(X,Y,Z,P,Q):- auxiliar1(X),atomo(Y),conectivo(Z),atomo(P),auxiliar2(Q).% exemplo teste: formula(/,p,>,q,\).
formula(W,X,Y,Z,P,Q):- negacao(W),auxiliar1(X),atomo(Y),conectivo(Z),atomo(P),auxiliar2(Q).% exemplo teste: formula(~,/,p,>,q,\).
formula(A,B,C,D,E,F) :- auxiliar1(A),negacao(F),atomo(B),conectivo(C),atomo(D),auxiliar2(E).
formula(A,B,C,D,E,F) :- auxiliar1(A),atomo(B),conectivo(C),negacao(F),atomo(D),auxiliar2(E).
formula(X,Y,Z,T,U,V,W) :- atomo(X),conectivo(Y),auxiliar1(Z),atomo(T),conectivo(U),atomo(V),auxiliar2(W).%exemplo teste: formula(p,>,/,p,#,q\).
formula(X,Y,Z,T,U,V,A,B,C,D,E) :- formula(X,Y,Z,T,U),conectivo(V), formula(A,B,C,D,E).% exemplo teste: formula(/,p,>,q,\,>,/,p,>,q,\)
formula(A,B,C,D,E,F,G,H,I,J,K,L) :- negacao(A),formula(B,C,D,E,F,G,H,I,J,K,L).
formula(A,B,C,D,E,F,G,H,I,J,K,L):- formula(A,B,C,D,E,F),conectivo(G),formula(H,I,J,K,L).
formula(A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,X,Y,Z):- formula(A,B,C,D,E,F,G,H,I,J,K,L),conectivo(M).formula(N,O,P,Q,R,S,T,U,V,X,Y,Z).
formula(A,B,C,D,E,F,G,H,I,J) :- formula(A,B,C,D,E,F,G), conectivo(H),formula(I,J).













